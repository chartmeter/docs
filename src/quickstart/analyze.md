# Analyze data

Once you have chart loaded and starred, you will be able to run SQL query with tabular data.

## Import chart as database table
Let's load chart table into database.

* Go back to **work** app, and click `Queries` panel tab on left under my space.
* Click `+` above query session list to open **console** app in new tab.
* Click `TABLES` dropdown and select `Import New` to open new table dialog.
* Select checkbox of `fruit sales` we just starred, and click `import`.
* Click `fruit sales` table, table schema displayed under `TABLE COLUMNS`

Congratulations, you just loaded chart table into database!

## Run query
Let's run a sample query.

```sql
SELECT t.fruit, SUM(t.sales) as total
FROM "fruit sales" AS t
GROUP BY t.fruit
```

* Copy SQL above, paste it in **SQL editor** and click `Run SQL`.
* Find query results under the editor.
* Click `Save As` icon in toolbar on top, left to `Run SQL`, and enter query session info.
    * Session name must be unique, let's say `fruit sales`.
    * Description is optional.
    * Click `Submit`.

Congratulations, you just created your first query session!

## Visualize
Let's visualize the query result.

* Click `brush` icon above query result to open an **embedded canvas**.
* Click `Choose Chart Type` button on top right corner and select `Pie`.
* Setup chart with panel on the right side.
    * In `General` tab, click `Dimensions` dropdown and select fruit. Click outside dropdown to close it.
    * In `General` tab, click `Measure` dropdown and select total.
    * Find the pie chart plot on the left side.
* Click `Save As` icon in toolbar on top, left to `Chart Type` button and enter canvas info.
    * Canvas name must be unique, let's say `fruit sales`.
    * Description is optional.
    * Click `Submit`.
    * Go back to `work` app and click `Canvases` panel tab on left under my space.
    * Click `refresh` icon above canvas list, find the canvas just created.

Congratulations, you just created your first canvas!
