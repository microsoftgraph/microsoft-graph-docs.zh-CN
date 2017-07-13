<span data-ttu-id="c4b7e-p110">使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。</span><span class="sxs-lookup"><span data-stu-id="c4b7e-p110">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。

<span data-ttu-id="c4b7e-164">**注意：**仅 **driveType** 为 `personal` 的 [驱动器](../resources/drive.md) 支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="c4b7e-164">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <span data-ttu-id="c4b7e-165">注解</span><span class="sxs-lookup"><span data-stu-id="c4b7e-165">Remarks</span></span>
<a id="remarks" class="xliff"></a>

* <span data-ttu-id="c4b7e-166">使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。</span><span class="sxs-lookup"><span data-stu-id="c4b7e-166">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="c4b7e-167">链接在项的共享权限中可见，可以由该项的所有者删除。</span><span class="sxs-lookup"><span data-stu-id="c4b7e-167">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="c4b7e-168">除非项已被签出，否则链接始终指向该项的最新版本（仅限 SharePoint）。</span><span class="sxs-lookup"><span data-stu-id="c4b7e-168">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
