---

skip_file: yes

---

# 歡迎來到創造建築伺服器網站儲存庫！
> 用於發布、儲存創造建築伺服器網站的文章！

### 如何創建一篇頁面？

一篇頁面應以 Markdown (`.md`) 格式來撰寫。

頁面的資料夾與檔案名會變成文章的子目錄與網站名，如：`docs/info.md`會產生出`https://my-website.com/docs/info/` 的網頁。

其中頁面開頭應**設置以下屬性**：

- `title`– 文章標題
- `menu_order`– 菜單順序
- `post_status`– 文章的狀態。允許的值：`publish`、`draft`、`pending`、`future`
- `post_excerpt`– 文章摘錄
- `post_date`– 要設置的發布日期。允許的格式：`2022-09-01`、`20:14:59`
- `comment_status`– 文章的評論狀態。允許的值：`open`、`closed`
- `page_template`– 為文章設置的頁面模板
- `stick_post`– 將文章標記為置頂。允許的值：`yes`標記為置頂，`no`取消置頂。
- `taxonomy`– 文章標籤、類別等分類法。對於自定義文章子類型，請使用自定義分類法名稱。
- `custom_fields`– 文章的自定義字段。
- `skip_file`– 跳過文章的發布。允許值：`yes`跳過文章。


以下為範例：
```yaml
---

title: 我是文章標題
menu_order: 1
post_status: publish
post_excerpt: 我是文章摘錄
taxonomy:
    category:
        - 類別1
        - 類別2
    post_tag:
        - 標籤1
        - 標籤2
custom_fields:
    field1: 自定義自段 1
    field2: value 2

---

## 我的文章的副標題
...
```

