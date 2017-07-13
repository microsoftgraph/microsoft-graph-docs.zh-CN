<span data-ttu-id="f61ba-p117">搜索条件使用高级查询语法 (AQS) 进行表示。结果按邮件发送日期和时间进行排序。</span><span class="sxs-lookup"><span data-stu-id="f61ba-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

搜索条件使用高级查询语法 (AQS) 进行表示。结果按邮件发送日期和时间进行排序。

<span data-ttu-id="f61ba-194">可以在 `$search` 条件中对 `message` 指定下列属性：`attachments`、`bccRecipients`、`body`、`category`、`ccRecipients`、`content`、`from`、`hasAttachments`、`participants`、`receivedDateTime`、`sender`、`subject`、`toRecipients`</span><span class="sxs-lookup"><span data-stu-id="f61ba-194">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="f61ba-195">如果要搜索邮件并且仅指定了一个值，那么会根据默认搜索属性 `from`、`subject` 和 `body` 进行搜索。</span><span class="sxs-lookup"><span data-stu-id="f61ba-195">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="f61ba-196">下面的示例返回登录用户收件箱中在三个默认搜索属性的任意一个中包含“pizza”的的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="f61ba-196">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="f61ba-197">下一个示例在用户收件箱中搜索从指定电子邮件地址发送的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="f61ba-197">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
