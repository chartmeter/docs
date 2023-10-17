# Quickstart
This guide covers how you can quickly get started using chartmeter

## Create a team workspace
A team space is required for any work in chartmeter.

* Open [`home page`] in browser.
* Click `Workspace` to open **work** app.
* Click `New Team Space` and enter space info.
    * Space name must be unique
    * Description is optional
    * Click `Submit`

Congratulations, you just created your first team space!

## Load data
### Create a collection
A collection is required for any chart.

* In **work** app, click `Charts` panel tab on left under team space.
* Click `+` above collection list and enter collection info.
    * Collection name must be unique in space.
    * Description is optional.
    * Click `Submit`.
    * Double click the collection you just created show up in the list.

Congratulations, You just created your first collection!

### Upload a chart
Let's create your first chart in collection by porting chart image. We will use [`fruit sales`] as sample.

* Click `+` above chart list to open **create chart** app in new tab.
* Download [`fruit sales`] image.
* Click `Upload` on top right corner and select `Image` to open upload dialog.
* Click `Chart Type` dropdown and select `Bar`.
* Select `muti-color series` checkbox.
* Click `Choose Image` and open the downloaded [`fruit sales`] image.
* Click `Submit` and wait till data decoded as table from image.

Congratulations, you just ported a chart image into tabular data!

### Edit and save table
Let's further edit table header.

* Click &#8942; icon next to *D0* and select `Edit Column` to open column dialog.
* Change column name from *D0* to *fruit* then click `Apply`.
* Further rename *D1* as *year* and *Est* as *sales*.
    * Now the table header should be *fruit*, *year* and *sales*.
    * We will use the new header name for SQL query later.
* Click `Save As` icon in toolbar, left to `Upload`, and enter chart info
    * Chart name must be unique in collection, let's say `fruit sales`
    * Description is optional
    * Click `Submit` and open **view chart** app in new tab
    * Click ⭐ icon in toolbar to *link chart into your personal space*, we will query it later.

Congratulations, you just created your first chart!

## Analyze data
Once you have chart loaded and starred, you will be able to run SQL query with tabular data.

### Import table
Let's load chart table into database.

* Go back to **work** app, and click `Queries` panel tab on left under my space.
* Click `+` above query session list to open **console** app in new tab.
* Click `TABLES` dropdown and select `Import New` to open new table dialog.
* Select checkbox of `fruit sales` we just starred, and click `import`.
* Click `fruit sales` table, table schema displayed under `TABLE COLUMNS`

Congratulations, you just loaded chart table into database!

### Run query
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

### Visualize
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

## Present data
With visualized data in canvas, it's time to showcase your data literacy.

### Create a channel
A channel is required for any post.

* In **work** app, click `Posts` panel tab on left under team space
* Click `+` above channel list and enter channel info.
    * Channel name must be unique in space.
    * Description is optional.
    * Channel handle must be unique for public channel.
    * Click `Submit`.
    * Double click the channel you just created show up in the list.

Congratulations, You just created your first channel!

### Create a post
Let's create a post in the channel.

* Click `+` above post list and enter post info.
    * Click `topic` dropdown and select a topic, or you can just type for autocomplete.
    * Post name must be unique in channel.
    * Post description is optional.
    * Click `Submit` and open post app in new tab.

Congratulations, you just created your first post!

### Compose
Let's add some content to your post.

* Click `New Slide` button and import your canvas
    * Select checkbox of `fruit sales`.
    * Both `Title` and `Subtitle` are required.
    * Click `Submit`.
    * You may find
        * New slide added to slide navigator panel on right side.
        * Your canvas imported as post chart on left side.
* Resize and move chart and text block
    * Resize by dragging bottom right corner of the block.
    * Move text block by dragging the empty header space left to `Delete` icon.
    * Move chart block by dragging empty space around the plot.
* Comments with editor in text block.
* Click `Save` to save your post.

Congratulations, you just compose your first post slide!

### Showcase
Once finish composing, let's share your post with others.

* Switch to post info panel on the right side by click `>>` then `info` icon
* Click `Submit` then `Publish` in overview section
    * You can either skip or follow hints
* Now your post is available to public
    * Make announcement with instant message by click `Send` icon in toolbar on top
    * Open post from public by click `Expo`

Congratulations, you just publish your first post to public!

[`home page`]: https://www.chart2char.com
[`fruit sales`]: misc/fruit%20sales.png
