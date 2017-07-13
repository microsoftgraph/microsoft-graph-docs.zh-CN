<span data-ttu-id="af0a8-p105">下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：</span><span class="sxs-lookup"><span data-stu-id="af0a8-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

下表定义了可能的缩略图大小。虽然可以请求任意的缩略图大小，但可能存在定义的有并迅速返回值：

| <span data-ttu-id="af0a8-162">名称</span><span class="sxs-lookup"><span data-stu-id="af0a8-162">Name</span></span>           | <span data-ttu-id="af0a8-163">分辨率</span><span class="sxs-lookup"><span data-stu-id="af0a8-163">Resolution</span></span>  | <span data-ttu-id="af0a8-164">纵横比​​</span><span class="sxs-lookup"><span data-stu-id="af0a8-164">Aspect Ratio</span></span> | <span data-ttu-id="af0a8-165">说明</span><span class="sxs-lookup"><span data-stu-id="af0a8-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="af0a8-166">96 longest</span><span class="sxs-lookup"><span data-stu-id="af0a8-166">96 longest</span></span>  | <span data-ttu-id="af0a8-167">Original</span><span class="sxs-lookup"><span data-stu-id="af0a8-167">Original</span></span>     | <span data-ttu-id="af0a8-168">小型的高压缩缩略图，裁剪为正方形纵横比。</span><span class="sxs-lookup"><span data-stu-id="af0a8-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="af0a8-169">176 longest</span><span class="sxs-lookup"><span data-stu-id="af0a8-169">176 longest</span></span> | <span data-ttu-id="af0a8-170">Original</span><span class="sxs-lookup"><span data-stu-id="af0a8-170">Original</span></span>     | <span data-ttu-id="af0a8-171">裁剪为 OneDrive Web 视图的标准项目大小。</span><span class="sxs-lookup"><span data-stu-id="af0a8-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="af0a8-172">800 longest
</span><span class="sxs-lookup"><span data-stu-id="af0a8-172">800 longest</span></span> | <span data-ttu-id="af0a8-173">Original</span><span class="sxs-lookup"><span data-stu-id="af0a8-173">Original</span></span>     | <span data-ttu-id="af0a8-174">最长边调整到 800 像素的缩略图。</span><span class="sxs-lookup"><span data-stu-id="af0a8-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <span data-ttu-id="af0a8-175">注解</span><span class="sxs-lookup"><span data-stu-id="af0a8-175">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="af0a8-176">**注意** 在 OneDrive for Business 和 SharePoint 中：</span><span class="sxs-lookup"><span data-stu-id="af0a8-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="af0a8-177">使用这些调用展开缩略图集合不适用于：`GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="af0a8-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
