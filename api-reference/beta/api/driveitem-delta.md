---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 同步驱动器的内容
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d93853ab0be35228bd7936b8c352d53d3c36f946
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589807"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="ecd4a-102">跟踪驱动器更改</span><span class="sxs-lookup"><span data-stu-id="ecd4a-102">Track changes for a Drive</span></span>

<span data-ttu-id="ecd4a-103">此方法使应用程序随着时间的推移跟踪驱动器及其子级的更改。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-103">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="ecd4a-p101">应用程序首先调用不带任何参数的 `delta`。服务开始枚举驱动器的层次结构，返回项目页面和 `@odata.nextLink` 或 `@odata.deltaLink`，如下所述。应用程序应该使用 `@odata.nextLink` 继续调用，直到不再返回 `@odata.nextLink`，或响应内容为空更改集。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="ecd4a-p102">接收完所有更改后，可将这些更改应用于本地状态。若要在将来检查更改，请通过上一响应中的 `@odata.deltaLink` 再次调用 `delta`。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="ecd4a-p103">返回具有 [`deleted` 方面](../resources/deleted.md) 的已删除邮件。应从本地状态中删除设置此属性的项目。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="ecd4a-111">**注意：** 如果在同步所有更改后文件夹为空，则仅应在本地删除此文件夹。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-111">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecd4a-112">权限</span><span class="sxs-lookup"><span data-stu-id="ecd4a-112">Permissions</span></span>

<span data-ttu-id="ecd4a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecd4a-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecd4a-115">Permission type</span></span>      | <span data-ttu-id="ecd4a-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ecd4a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecd4a-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecd4a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ecd4a-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecd4a-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ecd4a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecd4a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecd4a-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecd4a-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ecd4a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecd4a-121">Application</span></span> | <span data-ttu-id="ecd4a-122">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecd4a-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecd4a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecd4a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="ecd4a-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="ecd4a-124">Function parameters</span></span>

| <span data-ttu-id="ecd4a-125">参数</span><span class="sxs-lookup"><span data-stu-id="ecd4a-125">Parameter</span></span>   | <span data-ttu-id="ecd4a-126">类型</span><span class="sxs-lookup"><span data-stu-id="ecd4a-126">Type</span></span>  | <span data-ttu-id="ecd4a-127">说明</span><span class="sxs-lookup"><span data-stu-id="ecd4a-127">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ecd4a-128">令牌</span><span class="sxs-lookup"><span data-stu-id="ecd4a-128">token</span></span>  | <span data-ttu-id="ecd4a-129">字符串</span><span class="sxs-lookup"><span data-stu-id="ecd4a-129">string</span></span> | <span data-ttu-id="ecd4a-130">可选。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-130">Optional.</span></span> <span data-ttu-id="ecd4a-131">如果未指定，则枚举层次结构的当前状态。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-131">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="ecd4a-132">如果为 `latest`，则返回具有最新增量令牌的空响应。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-132">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="ecd4a-133">如果为之前的增量令牌，则返回自该令牌起的新状态。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-133">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ecd4a-134">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="ecd4a-134">Optional query parameters</span></span>

<span data-ttu-id="ecd4a-135">此方法支持使用 `$select`、`$expand` 和 `$top` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-135">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="ecd4a-136">响应</span><span class="sxs-lookup"><span data-stu-id="ecd4a-136">Response</span></span>

<span data-ttu-id="ecd4a-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItem](../resources/driveitem.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-137">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="ecd4a-138">除了 DriveItems 集合，此响应还包括以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="ecd4a-138">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="ecd4a-139">名称</span><span class="sxs-lookup"><span data-stu-id="ecd4a-139">Name</span></span>                 | <span data-ttu-id="ecd4a-140">值</span><span class="sxs-lookup"><span data-stu-id="ecd4a-140">Value</span></span>  | <span data-ttu-id="ecd4a-141">说明</span><span class="sxs-lookup"><span data-stu-id="ecd4a-141">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ecd4a-142">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="ecd4a-142">**@odata.nextLink**</span></span>  | <span data-ttu-id="ecd4a-143">url</span><span class="sxs-lookup"><span data-stu-id="ecd4a-143">url</span></span>    | <span data-ttu-id="ecd4a-144">如果当前集有其他更改，用来检索下一可用更改页的 URL。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-144">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="ecd4a-145">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="ecd4a-145">**@odata.deltaLink**</span></span> | <span data-ttu-id="ecd4a-146">url</span><span class="sxs-lookup"><span data-stu-id="ecd4a-146">url</span></span>    | <span data-ttu-id="ecd4a-p106">返回当前所有更改后返回的 URL，而不是 **@odata.nextLink**。用于在将来读取下一组更改。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p106">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="ecd4a-149">示例（初始请求）</span><span class="sxs-lookup"><span data-stu-id="ecd4a-149">Example (Initial Request)</span></span>

<span data-ttu-id="ecd4a-150">下面是一个如何调用此 API 以建立本地状态的示例。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-150">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="ecd4a-151">请求</span><span class="sxs-lookup"><span data-stu-id="ecd4a-151">Request</span></span>

<span data-ttu-id="ecd4a-152">下面是一个初始请求的示例。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-152">Here is an example of the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a><span data-ttu-id="ecd4a-153">响应</span><span class="sxs-lookup"><span data-stu-id="ecd4a-153">Response</span></span>

<span data-ttu-id="ecd4a-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-154">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ecd4a-155">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ecd4a-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ecd4a-156">C#</span><span class="sxs-lookup"><span data-stu-id="ecd4a-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_item_delta_first-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ecd4a-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="ecd4a-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_item_delta_first-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ecd4a-p107">此响应包含第一页的更改，**@odata.nextLink** 属性指示当前的项目集中有更多项目。在检索完所有项目页之前，你的应用程序应继续请求 **@odata.nextLink** 的 URL 值。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p107">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="ecd4a-160">示例（集中的最后一页）</span><span class="sxs-lookup"><span data-stu-id="ecd4a-160">Example (Last page in a set)</span></span>

<span data-ttu-id="ecd4a-161">下面是一个如何调用此 API 以更新本地状态的示例。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-161">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="ecd4a-162">请求</span><span class="sxs-lookup"><span data-stu-id="ecd4a-162">Request</span></span>

<span data-ttu-id="ecd4a-163">下面是一个初始请求之后的请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-163">Here is an example request after the initial request.</span></span>

<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a><span data-ttu-id="ecd4a-164">响应</span><span class="sxs-lookup"><span data-stu-id="ecd4a-164">Response</span></span>

<span data-ttu-id="ecd4a-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-165">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ecd4a-166">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ecd4a-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ecd4a-167">C#</span><span class="sxs-lookup"><span data-stu-id="ecd4a-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-item-delta-last-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ecd4a-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="ecd4a-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-item-delta-last-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ecd4a-169">此响应表示名为 `folder2` 的项目已被删除，并在初始请求和此请求之间添加或修改了 `file.txt` 项目以更新本地状态。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-169">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="ecd4a-170">最后一页的项目将包括 **@odata.deltaLink** 属性，此属性提供的 URL 以后可用于检索自当前项目集起的更改。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-170">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="ecd4a-p108">可能会发生本服务无法为特定标记提供更改列表的情况（例如，如果客户端在连接断开很长时间后尝试重新使用旧标记，或如果服务器状态已更改并需要新标记）。在这些情况下，本服务将返回带有错误响应的 `HTTP 410 Gone` 错误（包含以下错误代码之一）和 `Location` 标头（包含从头开始全新的增量枚举的新 nextLink）。完成全部枚举后，将返回的项目与本地状态进行比较，并遵循以下说明。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="ecd4a-174">错误类型</span><span class="sxs-lookup"><span data-stu-id="ecd4a-174">Error Type</span></span>                       | <span data-ttu-id="ecd4a-175">说明</span><span class="sxs-lookup"><span data-stu-id="ecd4a-175">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="ecd4a-p109">如果确定上次同步时服务与你的本地更改保持同步，请将任意本地项目替换为服务器的版本（包括删除）。上载服务器并不知道的任意本地更改。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="ecd4a-178">上载服务未返回的任意本地项目，并上载与服务器版本不同的任意文件（如果不知道哪个是最新的，请保留两份）。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-178">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="ecd4a-179">检索当前 deltaLink</span><span class="sxs-lookup"><span data-stu-id="ecd4a-179">Retrieving the current deltaLink</span></span>

<span data-ttu-id="ecd4a-180">在某些情况下，请求当前 deltaLink 值可能非常有用（无需首先枚举驱动器中已有的所有项）。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-180">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="ecd4a-181">如果应用只需了解更改，不需要了解现有项，这将非常有用。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-181">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="ecd4a-182">若要检索最新的 deltaLink，请使用查询字符串参数 `?token=latest` 调用 `delta`。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-182">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="ecd4a-183">**注意：若要尝试保持文件夹或驱动器中项的完整本地表示形式，必须使用 `delta` 进行初始枚举。如果在枚举期间发生任何写入操作，无法确保其他方法（如通过文件夹的 `children` 集合分页）返回所有项。使用 `delta` 是确保已读取所需全部数据的唯一方法。**</span><span class="sxs-lookup"><span data-stu-id="ecd4a-183">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="ecd4a-184">请求</span><span class="sxs-lookup"><span data-stu-id="ecd4a-184">Request</span></span>

<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a><span data-ttu-id="ecd4a-185">响应</span><span class="sxs-lookup"><span data-stu-id="ecd4a-185">Response</span></span>

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ecd4a-186">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ecd4a-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ecd4a-187">C#</span><span class="sxs-lookup"><span data-stu-id="ecd4a-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-delta-latest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ecd4a-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="ecd4a-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-delta-latest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="ecd4a-189">注解</span><span class="sxs-lookup"><span data-stu-id="ecd4a-189">Remarks</span></span>

* <span data-ttu-id="ecd4a-p111">增量源显示每项的最新状态，而不是每个更改的最新状态。如果项目重命名两次，它只显示一次并且使用最新名称。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="ecd4a-p112">出于各种原因，同一项可能在增量源中出现不止一次。你应使用最后一次出现的项目。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="ecd4a-p113">项目中的 `parentReference` 属性将不包括**路径**的值。之所以出现这种情况，是因为重命名文件夹不会导致从 **delta** 返回文件夹的任何后代。**使用增量时应始终按 id 跟踪项目**。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="ecd4a-197">在 OneDrive for Business 和 SharePoint 中，仅驱动器内的 `root` 文件夹支持 `delta`，其他文件夹并不支持。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-197">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="ecd4a-198">Delta 查询不会返回某些 DriveItem 属性，具体取决于操作和服务类型，如下表所示。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-198">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="ecd4a-199">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="ecd4a-199">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="ecd4a-200">操作类型</span><span class="sxs-lookup"><span data-stu-id="ecd4a-200">Operation type</span></span> | <span data-ttu-id="ecd4a-201">Delta 查询忽略的属性</span><span class="sxs-lookup"><span data-stu-id="ecd4a-201">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="ecd4a-202">创建/修改</span><span class="sxs-lookup"><span data-stu-id="ecd4a-202">Create/Modify</span></span> | <span data-ttu-id="ecd4a-203">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="ecd4a-203">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="ecd4a-204">删除</span><span class="sxs-lookup"><span data-stu-id="ecd4a-204">Delete</span></span> | <span data-ttu-id="ecd4a-205">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="ecd4a-205"></span></span> |


    <span data-ttu-id="ecd4a-206">**OneDrive（消费者）**</span><span class="sxs-lookup"><span data-stu-id="ecd4a-206">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="ecd4a-207">操作类型</span><span class="sxs-lookup"><span data-stu-id="ecd4a-207">Operation type</span></span> | <span data-ttu-id="ecd4a-208">Delta 查询忽略的属性</span><span class="sxs-lookup"><span data-stu-id="ecd4a-208">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="ecd4a-209">创建/修改</span><span class="sxs-lookup"><span data-stu-id="ecd4a-209">Create/Modify</span></span> | <span data-ttu-id="ecd4a-210">不适用</span><span class="sxs-lookup"><span data-stu-id="ecd4a-210">n/a</span></span> |
    | <span data-ttu-id="ecd4a-211">删除</span><span class="sxs-lookup"><span data-stu-id="ecd4a-211">Delete</span></span> | <span data-ttu-id="ecd4a-212">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="ecd4a-212"></span></span> |

## <a name="error-responses"></a><span data-ttu-id="ecd4a-213">错误响应</span><span class="sxs-lookup"><span data-stu-id="ecd4a-213">Error responses</span></span>

<span data-ttu-id="ecd4a-214">除了上面详述的重新同步错误之外，还请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="ecd4a-214">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
