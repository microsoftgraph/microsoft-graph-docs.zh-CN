# <a name="track-changes-for-a-drive"></a><span data-ttu-id="56428-101">跟踪驱动器更改</span><span class="sxs-lookup"><span data-stu-id="56428-101">Track changes for a Drive</span></span>

<span data-ttu-id="56428-102">此方法使应用程序随着时间的推移跟踪驱动器及其子级的更改。</span><span class="sxs-lookup"><span data-stu-id="56428-102">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="56428-p101">应用程序首先调用不带任何参数的 `delta`。服务开始枚举驱动器的层次结构，返回项目页面和 `@odata.nextLink` 或 `@odata.deltaLink`，如下所述。应用程序应该使用 `@odata.nextLink` 继续调用，直到不再返回 `@odata.nextLink`，或响应内容为空更改集。</span><span class="sxs-lookup"><span data-stu-id="56428-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="56428-p102">接收完所有更改后，可将这些更改应用于本地状态。若要在将来检查更改，请通过上一响应中的 `@odata.deltaLink` 再次调用 `delta`。</span><span class="sxs-lookup"><span data-stu-id="56428-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="56428-p103">返回具有 [`deleted` 方面](../resources/deleted.md) 的已删除邮件。应从本地状态中删除设置此属性的项目。</span><span class="sxs-lookup"><span data-stu-id="56428-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="56428-110">**注意：**如果在同步所有更改后文件夹为空，则仅应在本地删除此文件夹。</span><span class="sxs-lookup"><span data-stu-id="56428-110">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="56428-111">权限</span><span class="sxs-lookup"><span data-stu-id="56428-111">Permissions</span></span>
<span data-ttu-id="56428-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="56428-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56428-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="56428-114">Permission type</span></span>      | <span data-ttu-id="56428-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56428-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56428-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56428-116">Delegated (work or school account)</span></span> | <span data-ttu-id="56428-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56428-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="56428-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56428-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56428-119">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56428-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="56428-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="56428-120">Application</span></span> | <span data-ttu-id="56428-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56428-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56428-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56428-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/delta
GET /drives/{drive-id}/root/delta
GET /groups/{group-id}/drive/root/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56428-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56428-123">Optional query parameters</span></span>
<span data-ttu-id="56428-124">此方法支持使用 `$select`、`$expand` 和 `$top` [OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="56428-124">This method supports the `$select` and `$top` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="56428-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="56428-125">Request body</span></span>
<span data-ttu-id="56428-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56428-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56428-127">响应</span><span class="sxs-lookup"><span data-stu-id="56428-127">Response</span></span>

<span data-ttu-id="56428-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItem](../resources/driveitem.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="56428-128">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="56428-129">除了 DriveItems 集合，此响应还包括以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="56428-129">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="56428-130">名称</span><span class="sxs-lookup"><span data-stu-id="56428-130">Name</span></span>                 | <span data-ttu-id="56428-131">值</span><span class="sxs-lookup"><span data-stu-id="56428-131">Value</span></span>  | <span data-ttu-id="56428-132">说明</span><span class="sxs-lookup"><span data-stu-id="56428-132">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="56428-133">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="56428-133">**@odata.nextLink**</span></span>  | <span data-ttu-id="56428-134">url</span><span class="sxs-lookup"><span data-stu-id="56428-134">url</span></span>    | <span data-ttu-id="56428-135">如果当前集有其他更改，用来检索下一可用更改页的 URL。</span><span class="sxs-lookup"><span data-stu-id="56428-135">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="56428-136">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="56428-136">**@odata.deltaLink**</span></span> | <span data-ttu-id="56428-137">url</span><span class="sxs-lookup"><span data-stu-id="56428-137">url</span></span>    | <span data-ttu-id="56428-p105">返回当前所有更改后返回的 URL，而不是 **@odata.nextLink**。用于在将来读取下一组更改。</span><span class="sxs-lookup"><span data-stu-id="56428-p105">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="56428-140">示例（初始请求）</span><span class="sxs-lookup"><span data-stu-id="56428-140">Example (Initial Request)</span></span>
<span data-ttu-id="56428-141">下面是一个如何调用此 API 以建立本地状态的示例。</span><span class="sxs-lookup"><span data-stu-id="56428-141">Here is an example of how to call this API to establish your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="56428-142">请求</span><span class="sxs-lookup"><span data-stu-id="56428-142">Request</span></span>
<span data-ttu-id="56428-143">下面是一个初始请求的示例。</span><span class="sxs-lookup"><span data-stu-id="56428-143">Here is an example of the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

##### <a name="response"></a><span data-ttu-id="56428-144">响应</span><span class="sxs-lookup"><span data-stu-id="56428-144">Response</span></span>
<span data-ttu-id="56428-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="56428-145">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

<span data-ttu-id="56428-p106">此响应包含第一页的更改，**@odata.nextLink** 属性指示当前的项目集中有更多项目。在检索完所有项目页之前，你的应用程序应继续请求 **@odata.nextLink** 的 URL 值。</span><span class="sxs-lookup"><span data-stu-id="56428-p106">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="56428-148">示例（集中的最后一页）</span><span class="sxs-lookup"><span data-stu-id="56428-148">Example (Last page in a set)</span></span>
<span data-ttu-id="56428-149">下面是一个如何调用此 API 以更新本地状态的示例。</span><span class="sxs-lookup"><span data-stu-id="56428-149">Here is an example of how to call this API to update your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="56428-150">请求</span><span class="sxs-lookup"><span data-stu-id="56428-150">Request</span></span>
<span data-ttu-id="56428-151">下面是一个初始请求之后的请求示例。</span><span class="sxs-lookup"><span data-stu-id="56428-151">Here is an example request after the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

##### <a name="response"></a><span data-ttu-id="56428-152">响应</span><span class="sxs-lookup"><span data-stu-id="56428-152">Response</span></span>
<span data-ttu-id="56428-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="56428-153">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

<span data-ttu-id="56428-154">此响应表示名为 `folder2` 的项目已被删除，并在初始请求和此请求之间添加或修改了 `file.txt` 项目以更新本地状态。</span><span class="sxs-lookup"><span data-stu-id="56428-154">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="56428-155">最后一页的项目将包括 **@odata.deltaLink** 属性，此属性提供的 URL 以后可用于检索自当前项目集起的更改。</span><span class="sxs-lookup"><span data-stu-id="56428-155">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

## <a name="remarks"></a><span data-ttu-id="56428-156">注解</span><span class="sxs-lookup"><span data-stu-id="56428-156">Remarks</span></span>

* <span data-ttu-id="56428-p107">增量源显示每项的最新状态，而不是每个更改的最新状态。如果项目重命名两次，它只显示一次并且使用最新名称。</span><span class="sxs-lookup"><span data-stu-id="56428-p107">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="56428-p108">出于各种原因，同一项可能在增量源中出现不止一次。你应使用最后一次出现的项目。</span><span class="sxs-lookup"><span data-stu-id="56428-p108">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="56428-p109">项目中的 `parentReference` 属性将不包括**路径**的值。之所以出现这种情况，是因为重命名文件夹不会导致从 **delta** 返回文件夹的任何后代。**使用增量时应始终按 id 跟踪项目**。</span><span class="sxs-lookup"><span data-stu-id="56428-p109">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>

<span data-ttu-id="56428-p110">可能会发生本服务无法为特定标记提供更改列表的情况（例如，如果客户端在连接断开很长时间后尝试重新使用旧标记，或如果服务器状态已更改并需要新标记）。在这些情况下，本服务将返回带有错误响应的 `HTTP 410 Gone` 错误（包含以下错误代码之一）和 `Location` 标头（包含从头开始全新的增量枚举的新 nextLink）。完成全部枚举后，将返回的项目与本地状态进行比较，并遵循以下说明。</span><span class="sxs-lookup"><span data-stu-id="56428-p110">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="56428-167">错误类型</span><span class="sxs-lookup"><span data-stu-id="56428-167">Error Type</span></span>                       | <span data-ttu-id="56428-168">说明</span><span class="sxs-lookup"><span data-stu-id="56428-168">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="56428-p111">如果确定上次同步时服务与你的本地更改保持同步，请将任意本地项目替换为服务器的版本（包括删除）。上载服务器并不知道的任意本地更改。</span><span class="sxs-lookup"><span data-stu-id="56428-p111">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="56428-171">上载服务未返回的任意本地项目，并上载与服务器版本不同的任意文件（如果不知道哪个是最新的，请保留两份）。</span><span class="sxs-lookup"><span data-stu-id="56428-171">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

<span data-ttu-id="56428-p112">在 OneDrive for Business 和 SharePoint 中，仅 `root` 文件夹支持 `delta`，其他文件夹并不支持。它也不会返回以下 DriveItem 属性：</span><span class="sxs-lookup"><span data-stu-id="56428-p112">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders. It also will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="56428-174">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="56428-174">**createdBy**</span></span>
* <span data-ttu-id="56428-175">**cTag**</span><span class="sxs-lookup"><span data-stu-id="56428-175">**cTag**</span></span>
* <span data-ttu-id="56428-176">**eTag**</span><span class="sxs-lookup"><span data-stu-id="56428-176">**eTag**</span></span>
* <span data-ttu-id="56428-177">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="56428-177">**fileSystemInfo**</span></span>
* <span data-ttu-id="56428-178">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="56428-178">**lastModifiedBy**</span></span>
* <span data-ttu-id="56428-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="56428-179">**parentReference**</span></span>
* <span data-ttu-id="56428-180">**size**</span><span class="sxs-lookup"><span data-stu-id="56428-180">**size**</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "Get item delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
