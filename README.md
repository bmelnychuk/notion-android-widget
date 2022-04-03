# Notion Todo List
Android home screen widget to display todo list from the notion (Tasker + KWGT)

I am using notion to organize many things in my life. Action Items List (or todo list) is the feature I use daily, so I wanted to have it always with me. Naturally, I wanted to see it as a widget on my phone's home screen. Unfortunately, I did not find any existing solution that does something similar, so I decided to do it myself.

 ### The final result
 <img src="https://github.com/bmelnychuk/notion-android-widget/blob/main/preview.jpg" width="400">
 
- Resizable home screen widget that renders todo list
- Navigation between pages (< >)
- Color to highlight the priority
- Click event to force a refresh

### Required android apps:
- [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en&gl=US): to organize the data fetching from the notion
- [KWGT](https://play.google.com/store/apps/details?id=org.kustom.widget): the widget builder
- [AutoTools](https://play.google.com/store/apps/details?id=com.joaomgcd.autotools): simplify the data parsing

I am not sure if any paid versions are required since I paid a long time ago.

For now, I will not describe in detail how to configure it. Everything is shared as-is. Feel free to contribute with step-by-step instructions.

### How to:
1) Create a table in the notion that follows the [schema](files/notion_table_schema.json)
2) Create an [integration](https://developers.notion.com/docs/getting-started) for the table
3) Install required android apps
4) Import [Tasker](files/NotionTodo.tsk.xml) and [KWGT](files/Notion_Todo_List_Clean.kwgt) files. Make sure you update `your_database_id` and `your_secret_token` token
5) Add the widget to the home screen


