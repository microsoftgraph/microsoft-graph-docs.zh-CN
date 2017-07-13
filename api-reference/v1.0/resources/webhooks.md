<span data-ttu-id="3459f-p119">将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。如果 Microsoft Graph 没有收到 2xx 类代码，它将重试多次发送通知。</span><span class="sxs-lookup"><span data-stu-id="3459f-p119">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
3. 将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。如果 Microsoft Graph 没有收到 2xx 类代码，它将重试多次发送通知。
  > <span data-ttu-id="3459f-198">即使 clientState 属性与订阅请求提交的属性不匹配，也应发送 `202 - Accepted` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="3459f-198">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="3459f-199">对请求中的其他通知重复该过程。</span><span class="sxs-lookup"><span data-stu-id="3459f-199">Repeat for other notifications in the request.</span></span>

# <span data-ttu-id="3459f-200">其他资源</span><span class="sxs-lookup"><span data-stu-id="3459f-200">Additional resources</span></span>
<a id="additional-resources" class="xliff"></a>

* [<span data-ttu-id="3459f-201">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="3459f-201">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="3459f-202">获取订阅</span><span class="sxs-lookup"><span data-stu-id="3459f-202">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="3459f-203">创建订阅</span><span class="sxs-lookup"><span data-stu-id="3459f-203">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* <span data-ttu-id="3459f-204">[Microsoft Graph Webhooks Sample for Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)（面向 Node.js 的 Microsoft Graph Webhooks 示例）</span><span class="sxs-lookup"><span data-stu-id="3459f-204">[Microsoft Graph Webhooks Sample for Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)</span></span>
* <span data-ttu-id="3459f-205">[Microsoft Graph Webhooks Sample for ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)（面向 ASP.NET 的 Microsoft Graph Webhooks 示例）</span><span class="sxs-lookup"><span data-stu-id="3459f-205">[Microsoft Graph Webhooks Sample for ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)</span></span>
