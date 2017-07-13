<span data-ttu-id="a04c0-p116">还需要对特定资源执行读取或写入操作所需的相同[权限](./permissions_reference.md)，以便对该资源上的任意扩展数据执行读取或写入操作。例如，对于能够使用自定义应用数据更新登录用户的个人资料的应用，必须向该应用授予 * User.ReadWrite.All * 权限。</span><span class="sxs-lookup"><span data-stu-id="a04c0-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

还需要对特定资源执行读取或写入操作所需的相同[权限](./permissions_reference.md)，以便对该资源上的任意扩展数据执行读取或写入操作。例如，对于能够使用自定义应用数据更新登录用户的个人资料的应用，必须向该应用授予 * User.ReadWrite.All * 权限。

<span data-ttu-id="a04c0-229">此外，要创建和管理架构扩展定义，必须向应用程序授予 *Directory.AccessAsUser.All* 权限。</span><span class="sxs-lookup"><span data-stu-id="a04c0-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <span data-ttu-id="a04c0-230">数据限制</span><span class="sxs-lookup"><span data-stu-id="a04c0-230">Data limits</span></span>
<a id="data-limits" class="xliff"></a>

### <span data-ttu-id="a04c0-231">开放扩展限制</span><span class="sxs-lookup"><span data-stu-id="a04c0-231">Open extension limits</span></span>
<a id="open-extension-limits" class="xliff"></a>
<span data-ttu-id="a04c0-232">以下限制适用于目录资源（如**用户**、**组**、**设备**）：</span><span class="sxs-lookup"><span data-stu-id="a04c0-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="a04c0-233">每个开放扩展最多可以包含 2KB 的数据（包括扩展定义本身）。</span><span class="sxs-lookup"><span data-stu-id="a04c0-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="a04c0-234">应用程序最多可为每个资源实例添加两个开放扩展。</span><span class="sxs-lookup"><span data-stu-id="a04c0-234">An application can add up to two open extensions per resource instance.</span></span>

### <span data-ttu-id="a04c0-235">架构扩展限制</span><span class="sxs-lookup"><span data-stu-id="a04c0-235">Schema extension limits</span></span>
<a id="schema-extension-limits" class="xliff"></a>
<span data-ttu-id="a04c0-236">应用程序最多可以创建五个**架构扩展**定义。</span><span class="sxs-lookup"><span data-stu-id="a04c0-236">An application may create no more than five **schema extension** definitions.</span></span>

## <span data-ttu-id="a04c0-237">已知限制</span><span class="sxs-lookup"><span data-stu-id="a04c0-237">Known limitations</span></span>
<a id="known-limitations" class="xliff"></a>

<span data-ttu-id="a04c0-238">有关使用扩展的已知限制，请参阅已知问题文章中的[扩展部分](known_issues.md#extensions)。</span><span class="sxs-lookup"><span data-stu-id="a04c0-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <span data-ttu-id="a04c0-239">扩展示例</span><span class="sxs-lookup"><span data-stu-id="a04c0-239">Extension examples</span></span>
<a id="extension-examples" class="xliff"></a>

[<span data-ttu-id="a04c0-240">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a04c0-240">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

[<span data-ttu-id="a04c0-241">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a04c0-241">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

## <span data-ttu-id="a04c0-242">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a04c0-242">See also</span></span>
<a id="see-also" class="xliff"></a>

<span data-ttu-id="a04c0-243">
  [Office 365 域](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="a04c0-243">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>

[<span data-ttu-id="a04c0-244">添加并验证 Office 365 租户的域</span><span class="sxs-lookup"><span data-stu-id="a04c0-244">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
