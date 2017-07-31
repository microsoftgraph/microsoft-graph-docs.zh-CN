<span data-ttu-id="ad934-p119">既然你已经了解如何调用 Microsoft Graph，现在就可以使用 API 参考来构造应用需要执行的其他任何种类调用。不过，请注意，应用需要获得应用注册时配置的适当权限，才能执行调用。</span><span class="sxs-lookup"><span data-stu-id="ad934-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

既然你已经了解如何调用 Microsoft Graph，现在就可以使用 API 参考来构造应用需要执行的其他任何种类调用。不过，请注意，应用需要获得应用注册时配置的适当权限，才能执行调用。

## <a name="next-steps"></a><span data-ttu-id="ad934-189">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ad934-189">Next steps</span></span>
- <span data-ttu-id="ad934-190">使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer) 试用更多 REST API。</span><span class="sxs-lookup"><span data-stu-id="ad934-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="ad934-191">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ad934-191">See also</span></span>
- [<span data-ttu-id="ad934-192">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="ad934-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="ad934-193">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="ad934-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
