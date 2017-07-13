<span data-ttu-id="6a2bd-p103">从 **sharedWithMe** 操作返回的 driveItem 始终都将包括 [**remoteItem**](../resources/remoteitem.md) 方面，这表明它们是其他驱动器中的项目。若要访问共享的 DriveItem 资源，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="6a2bd-p103">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

从 **sharedWithMe** 操作返回的 driveItem 始终都将包括 [**remoteItem**](../resources/remoteitem.md) 方面，这表明它们是其他驱动器中的项目。若要访问共享的 DriveItem 资源，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
