<span data-ttu-id="e1d79-p119">既然你已经了解如何调用 Microsoft Graph，现在就可以使用 API 参考来构造应用需要执行的其他任何种类调用。不过，请注意，应用需要获得应用注册时配置的适当权限，才能执行调用。</span><span class="sxs-lookup"><span data-stu-id="e1d79-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

既然你已经了解如何调用 Microsoft Graph，现在就可以使用 API 参考来构造应用需要执行的其他任何种类调用。不过，请注意，应用需要获得应用注册时配置的适当权限，才能执行调用。

## <a name="next-steps"></a><span data-ttu-id="e1d79-189">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e1d79-189">Next steps</span></span>
- <span data-ttu-id="e1d79-190">使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer) 试用更多 REST API。</span><span class="sxs-lookup"><span data-stu-id="e1d79-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="e1d79-191">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e1d79-191">See also</span></span>
- [<span data-ttu-id="e1d79-192">获取访问令牌以调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e1d79-192">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="e1d79-193">代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="e1d79-193">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="e1d79-194">不代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="e1d79-194">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
