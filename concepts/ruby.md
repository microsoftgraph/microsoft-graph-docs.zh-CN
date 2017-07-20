<span data-ttu-id="29f6c-p119">若要创建电子邮件，代码会通过窗体传递的参数中的会话令牌和收件人电子邮件地址拉取用户名。然后代码会在项目所包含的模板中读取电子邮件正文，插入用户名和电子邮件地址，并将电子邮件文本附加为 HTTP 请求正文。</span><span class="sxs-lookup"><span data-stu-id="29f6c-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

若要创建电子邮件，代码会通过窗体传递的参数中的会话令牌和收件人电子邮件地址拉取用户名。然后代码会在项目所包含的模板中读取电子邮件正文，插入用户名和电子邮件地址，并将电子邮件文本附加为 HTTP 请求正文。

<span data-ttu-id="29f6c-194">若要发送电子邮件，代码会构建 HTTP 请求，将访问令牌附加为授权标头，然后将请求发布至发送电子邮件终结点。</span><span class="sxs-lookup"><span data-stu-id="29f6c-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="29f6c-195">最后，代码会使用返回的 HTTP 响应代码来通知用户电子邮件是否发送成功。</span><span class="sxs-lookup"><span data-stu-id="29f6c-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="29f6c-196">运行应用</span><span class="sxs-lookup"><span data-stu-id="29f6c-196">Run the app</span></span>

1. <span data-ttu-id="29f6c-197">使用以下命令安装 Rails 应用程序和依存关系。</span><span class="sxs-lookup"><span data-stu-id="29f6c-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="29f6c-198">要启动 Rails 应用程序，请键入以下命令。</span><span class="sxs-lookup"><span data-stu-id="29f6c-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="29f6c-199">转到 Web 浏览器中的 `http://localhost:3000`。</span><span class="sxs-lookup"><span data-stu-id="29f6c-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="29f6c-200">另请参阅</span><span class="sxs-lookup"><span data-stu-id="29f6c-200">See also</span></span>
- <span data-ttu-id="29f6c-201">使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="29f6c-201">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="29f6c-202">在 GitHub 上浏览其他 [Microsoft Graph 示例](https://github.com/microsoftgraph)。</span><span class="sxs-lookup"><span data-stu-id="29f6c-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>
- [<span data-ttu-id="29f6c-203">获取访问令牌以调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="29f6c-203">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="29f6c-204">代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="29f6c-204">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="29f6c-205">不代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="29f6c-205">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)


