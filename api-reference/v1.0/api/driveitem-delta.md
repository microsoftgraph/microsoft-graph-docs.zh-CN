---
author: JeremyKelley
ms.date: 09/10/2017
title: 同步驱动器的内容
localization_priority: Priority
ms.prod: sharepoint
description: 此方法使应用程序随着时间的推移跟踪驱动器及其子级的更改。
doc_type: apiPageType
ms.openlocfilehash: bcf638e5217768012a7e361ebed3cd760ac079c0
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911310"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="10bea-103">跟踪驱动器更改</span><span class="sxs-lookup"><span data-stu-id="10bea-103">Track changes for a Drive</span></span>

<span data-ttu-id="10bea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10bea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10bea-105">此方法使应用程序随着时间的推移跟踪驱动器及其子级的更改。</span><span class="sxs-lookup"><span data-stu-id="10bea-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="10bea-p101">应用程序首先调用不带任何参数的 `delta`。服务开始枚举驱动器的层次结构，返回项目页面和 `@odata.nextLink` 或 `@odata.deltaLink`，如下所述。应用程序应该使用 `@odata.nextLink` 继续调用，直到不再返回 `@odata.nextLink`，或响应内容为空更改集。</span><span class="sxs-lookup"><span data-stu-id="10bea-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="10bea-p102">接收完所有更改后，可将这些更改应用于本地状态。若要在将来检查更改，请通过上一响应中的 `@odata.deltaLink` 再次调用 `delta`。</span><span class="sxs-lookup"><span data-stu-id="10bea-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="10bea-p103">返回具有 [`deleted` 方面](../resources/deleted.md) 的已删除邮件。应从本地状态中删除设置此属性的项目。</span><span class="sxs-lookup"><span data-stu-id="10bea-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

><span data-ttu-id="10bea-113">**注意：** 如果在同步所有更改后文件夹为空，则仅应在本地删除此文件夹。</span><span class="sxs-lookup"><span data-stu-id="10bea-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="10bea-114">权限</span><span class="sxs-lookup"><span data-stu-id="10bea-114">Permissions</span></span>

<span data-ttu-id="10bea-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10bea-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10bea-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="10bea-117">Permission type</span></span>      | <span data-ttu-id="10bea-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10bea-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10bea-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10bea-119">Delegated (work or school account)</span></span> | <span data-ttu-id="10bea-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bea-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="10bea-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10bea-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10bea-122">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bea-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="10bea-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="10bea-123">Application</span></span> | <span data-ttu-id="10bea-124">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bea-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10bea-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10bea-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="10bea-126">函数参数</span><span class="sxs-lookup"><span data-stu-id="10bea-126">Function parameters</span></span>

| <span data-ttu-id="10bea-127">参数</span><span class="sxs-lookup"><span data-stu-id="10bea-127">Parameter</span></span>   | <span data-ttu-id="10bea-128">类型</span><span class="sxs-lookup"><span data-stu-id="10bea-128">Type</span></span>  | <span data-ttu-id="10bea-129">说明</span><span class="sxs-lookup"><span data-stu-id="10bea-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="10bea-130">令牌</span><span class="sxs-lookup"><span data-stu-id="10bea-130">token</span></span>  | <span data-ttu-id="10bea-131">字符串</span><span class="sxs-lookup"><span data-stu-id="10bea-131">string</span></span> | <span data-ttu-id="10bea-132">可选。</span><span class="sxs-lookup"><span data-stu-id="10bea-132">Optional.</span></span> <span data-ttu-id="10bea-133">如果未指定，则枚举层次结构的当前状态。</span><span class="sxs-lookup"><span data-stu-id="10bea-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="10bea-134">如果为 `latest`，则返回具有最新增量令牌的空响应。</span><span class="sxs-lookup"><span data-stu-id="10bea-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="10bea-135">如果为之前的增量令牌，则返回自该令牌起的新状态。</span><span class="sxs-lookup"><span data-stu-id="10bea-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="10bea-136">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="10bea-136">Optional query parameters</span></span>

<span data-ttu-id="10bea-137">此方法支持使用 `$select`、`$expand` 和 `$top` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10bea-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="10bea-138">响应</span><span class="sxs-lookup"><span data-stu-id="10bea-138">Response</span></span>

<span data-ttu-id="10bea-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItem](../resources/driveitem.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="10bea-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="10bea-140">除了 DriveItems 集合，此响应还包括以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="10bea-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="10bea-141">名称</span><span class="sxs-lookup"><span data-stu-id="10bea-141">Name</span></span>                 | <span data-ttu-id="10bea-142">值</span><span class="sxs-lookup"><span data-stu-id="10bea-142">Value</span></span>  | <span data-ttu-id="10bea-143">说明</span><span class="sxs-lookup"><span data-stu-id="10bea-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="10bea-144">**\@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="10bea-144">**\@odata.nextLink**</span></span>  | <span data-ttu-id="10bea-145">url</span><span class="sxs-lookup"><span data-stu-id="10bea-145">url</span></span>    | <span data-ttu-id="10bea-146">如果当前集有其他更改，用来检索下一可用更改页的 URL。</span><span class="sxs-lookup"><span data-stu-id="10bea-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="10bea-147">**\@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="10bea-147">**\@odata.deltaLink**</span></span> | <span data-ttu-id="10bea-148">url</span><span class="sxs-lookup"><span data-stu-id="10bea-148">url</span></span>    | <span data-ttu-id="10bea-p106">返回当前所有更改后返回 URL，而不是 **\@odata.nextLink**。用于在将来读取下一组更改。</span><span class="sxs-lookup"><span data-stu-id="10bea-p106">A URL returned instead of **\@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="10bea-151">示例（初始请求）</span><span class="sxs-lookup"><span data-stu-id="10bea-151">Example (Initial Request)</span></span>

<span data-ttu-id="10bea-152">下面是一个如何调用此 API 以建立本地状态的示例。</span><span class="sxs-lookup"><span data-stu-id="10bea-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="10bea-153">请求</span><span class="sxs-lookup"><span data-stu-id="10bea-153">Request</span></span>

<span data-ttu-id="10bea-154">下面是一个初始请求的示例。</span><span class="sxs-lookup"><span data-stu-id="10bea-154">Here is an example of the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10bea-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bea-155">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="c"></a>[<span data-ttu-id="10bea-156">C#</span><span class="sxs-lookup"><span data-stu-id="10bea-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bea-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bea-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bea-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bea-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10bea-159">Java</span><span class="sxs-lookup"><span data-stu-id="10bea-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10bea-160">响应</span><span class="sxs-lookup"><span data-stu-id="10bea-160">Response</span></span>

<span data-ttu-id="10bea-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="10bea-161">Here is an example of the response.</span></span>

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

<span data-ttu-id="10bea-p107">此响应包含第一页的更改，**\@odata.nextLink** 属性指示当前的项目集中有更多项目。在检索完所有项目页之前，你的应用程序应继续请求 **\@odata.nextLink** 的 URL 值。</span><span class="sxs-lookup"><span data-stu-id="10bea-p107">This response includes the first page of changes, and the **\@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **\@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="10bea-164">示例（集中的最后一页）</span><span class="sxs-lookup"><span data-stu-id="10bea-164">Example (Last page in a set)</span></span>

<span data-ttu-id="10bea-165">下面是一个如何调用此 API 以更新本地状态的示例。</span><span class="sxs-lookup"><span data-stu-id="10bea-165">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="10bea-166">请求</span><span class="sxs-lookup"><span data-stu-id="10bea-166">Request</span></span>

<span data-ttu-id="10bea-167">下面是一个初始请求之后的请求示例。</span><span class="sxs-lookup"><span data-stu-id="10bea-167">Here is an example request after the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10bea-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bea-168">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[<span data-ttu-id="10bea-169">C#</span><span class="sxs-lookup"><span data-stu-id="10bea-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bea-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bea-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bea-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bea-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10bea-172">Java</span><span class="sxs-lookup"><span data-stu-id="10bea-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10bea-173">响应</span><span class="sxs-lookup"><span data-stu-id="10bea-173">Response</span></span>

<span data-ttu-id="10bea-174">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="10bea-174">Here is an example of the response.</span></span>

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

<span data-ttu-id="10bea-175">此响应表示名为 `folder2` 的项目已被删除，并在初始请求和此请求之间添加或修改了 `file.txt` 项目以更新本地状态。</span><span class="sxs-lookup"><span data-stu-id="10bea-175">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="10bea-176">最后一页的项目将包括 **\@odata.deltaLink** 属性，此属性提供的 URL 以后可用于检索自当前项目集以来的更改。</span><span class="sxs-lookup"><span data-stu-id="10bea-176">The final page of items will include the **\@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="10bea-p108">可能会发生本服务无法为特定标记提供更改列表的情况（例如，如果客户端在连接断开很长时间后尝试重新使用旧标记，或如果服务器状态已更改并需要新标记）。在这些情况下，本服务将返回带有错误响应的 `HTTP 410 Gone` 错误（包含以下错误代码之一）和 `Location` 标头（包含从头开始全新的增量枚举的新 nextLink）。完成全部枚举后，将返回的项目与本地状态进行比较，并遵循以下说明。</span><span class="sxs-lookup"><span data-stu-id="10bea-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="10bea-180">错误类型</span><span class="sxs-lookup"><span data-stu-id="10bea-180">Error Type</span></span>                       | <span data-ttu-id="10bea-181">说明</span><span class="sxs-lookup"><span data-stu-id="10bea-181">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="10bea-p109">如果确定上次同步时服务与你的本地更改保持同步，请将任意本地项目替换为服务器的版本（包括删除）。上载服务器并不知道的任意本地更改。</span><span class="sxs-lookup"><span data-stu-id="10bea-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="10bea-184">上载服务未返回的任意本地项目，并上载与服务器版本不同的任意文件（如果不知道哪个是最新的，请保留两份）。</span><span class="sxs-lookup"><span data-stu-id="10bea-184">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="10bea-185">检索当前 deltaLink</span><span class="sxs-lookup"><span data-stu-id="10bea-185">Retrieving the current deltaLink</span></span>

<span data-ttu-id="10bea-186">在某些情况下，请求当前 deltaLink 值可能非常有用（无需首先枚举驱动器中已有的所有项）。</span><span class="sxs-lookup"><span data-stu-id="10bea-186">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="10bea-p110">如果应用只需了解更改，不需要了解现有项，这将非常有用。若要检索最新的 deltaLink，请使用查询字符串参数 `?token=latest` 调用 `delta`。</span><span class="sxs-lookup"><span data-stu-id="10bea-p110">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items. To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="10bea-189">**注意：若要尝试保持文件夹或驱动器中项的完整本地表示形式，必须使用 `delta` 进行初始枚举。如果在枚举期间发生任何写入操作，无法确保其他方法（如通过文件夹的 `children` 集合分页）返回所有项。使用 `delta` 是确保已读取所需全部数据的唯一方法。**</span><span class="sxs-lookup"><span data-stu-id="10bea-189">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="10bea-190">请求</span><span class="sxs-lookup"><span data-stu-id="10bea-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="10bea-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bea-191">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[<span data-ttu-id="10bea-192">C#</span><span class="sxs-lookup"><span data-stu-id="10bea-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bea-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bea-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bea-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bea-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10bea-195">Java</span><span class="sxs-lookup"><span data-stu-id="10bea-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10bea-196">响应</span><span class="sxs-lookup"><span data-stu-id="10bea-196">Response</span></span>

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="10bea-197">注解</span><span class="sxs-lookup"><span data-stu-id="10bea-197">Remarks</span></span>

* <span data-ttu-id="10bea-p111">增量源显示每项的最新状态，而不是每个更改的最新状态。如果项目重命名两次，它只显示一次并且使用最新名称。</span><span class="sxs-lookup"><span data-stu-id="10bea-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="10bea-p112">出于各种原因，同一项可能在增量源中出现不止一次。你应使用最后一次出现的项目。</span><span class="sxs-lookup"><span data-stu-id="10bea-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="10bea-p113">项目中的 `parentReference` 属性将不包括 **路径** 的值。之所以出现这种情况，是因为重命名文件夹不会导致从 **delta** 返回文件夹的任何后代。**使用增量时应始终按 id 跟踪项目**。</span><span class="sxs-lookup"><span data-stu-id="10bea-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="10bea-205">Delta 查询不会返回某些 DriveItem 属性，具体取决于操作和服务类型，如下表所示。</span><span class="sxs-lookup"><span data-stu-id="10bea-205">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="10bea-206">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="10bea-206">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="10bea-207">操作类型</span><span class="sxs-lookup"><span data-stu-id="10bea-207">Operation type</span></span> | <span data-ttu-id="10bea-208">Delta 查询忽略的属性</span><span class="sxs-lookup"><span data-stu-id="10bea-208">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="10bea-209">创建/修改</span><span class="sxs-lookup"><span data-stu-id="10bea-209">Create/Modify</span></span> | <span data-ttu-id="10bea-210">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="10bea-210">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="10bea-211">删除</span><span class="sxs-lookup"><span data-stu-id="10bea-211">Delete</span></span> | <span data-ttu-id="10bea-212">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="10bea-212">`ctag`, `lastModifiedBy`, `name`</span></span> |


    <span data-ttu-id="10bea-213">**OneDrive（消费者）**</span><span class="sxs-lookup"><span data-stu-id="10bea-213">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="10bea-214">操作类型</span><span class="sxs-lookup"><span data-stu-id="10bea-214">Operation type</span></span> | <span data-ttu-id="10bea-215">Delta 查询忽略的属性</span><span class="sxs-lookup"><span data-stu-id="10bea-215">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="10bea-216">创建/修改</span><span class="sxs-lookup"><span data-stu-id="10bea-216">Create/Modify</span></span> | <span data-ttu-id="10bea-217">不适用</span><span class="sxs-lookup"><span data-stu-id="10bea-217">n/a</span></span> |
    | <span data-ttu-id="10bea-218">删除</span><span class="sxs-lookup"><span data-stu-id="10bea-218">Delete</span></span> | <span data-ttu-id="10bea-219">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="10bea-219">`ctag`, `size`</span></span> |

## <a name="scanning-permissions-hierarchies"></a><span data-ttu-id="10bea-220">扫描权限层次结构</span><span class="sxs-lookup"><span data-stu-id="10bea-220">Scanning permissions hierarchies</span></span>
<span data-ttu-id="10bea-221">默认情况下，增量查询响应将包含查询中所有项目的发生了更改的共享信息，即使这些项目从其父级继承了权限，本身没有直接的共享更改。</span><span class="sxs-lookup"><span data-stu-id="10bea-221">By default, the delta query response will include sharing information for all items in the query that changed even if they inherit their permissions from their parent and did not have direct sharing changes themselves.</span></span> <span data-ttu-id="10bea-222">这通常会导致执行后续调用，以便获取每个项目（而不仅仅是共享信息发生了更改的项目）的权限详细信息。</span><span class="sxs-lookup"><span data-stu-id="10bea-222">This typically then results in a follow up call to get the permission details for every item rather than just the ones whose sharing information changed.</span></span> <span data-ttu-id="10bea-223">通过向增量查询请求添加 `Prefer: hierarchicalsharing` 标头，能够帮助你更好地了解权限更改的发生方式。</span><span class="sxs-lookup"><span data-stu-id="10bea-223">You can optimize your understanding of how permission changes happen by adding the `Prefer: hierarchicalsharing` header to your delta query request.</span></span>

<span data-ttu-id="10bea-224">如果提供了 `Prefer: hierarchicalsharing` 标头，将返回以下对象的共享信息：权限层次结构的根以及明确具有共享更改的项目。</span><span class="sxs-lookup"><span data-stu-id="10bea-224">When the `Prefer: hierarchicalsharing` header is provided, sharing information will be returned for the root of the permissions hierarchy, as well as items that explicitly have sharing changes.</span></span> <span data-ttu-id="10bea-225">如果共享更改是从某个项目中删除共享，你会发现一个空的共享 facet，用以区分从其父级继承的项目和唯一但没有共享链接的项目。</span><span class="sxs-lookup"><span data-stu-id="10bea-225">In cases where the sharing change is to remove sharing from an item, you will find an empty sharing facet to differentiate between items that inherit from their parent and those that are unique but have no sharing links.</span></span> <span data-ttu-id="10bea-226">你还将在未共享用于建立初始作用域的权限层次结构的根处看到这个空的共享 facet。</span><span class="sxs-lookup"><span data-stu-id="10bea-226">You will also see this empty sharing facet on the root of a permission hierarchy that is not shared to establish the initial scope.</span></span>

<span data-ttu-id="10bea-227">在许多扫描场景中，你可能会对权限的更改特别感兴趣。</span><span class="sxs-lookup"><span data-stu-id="10bea-227">In many scanning scenarios, you might be interested specifically in changes to permissions.</span></span> <span data-ttu-id="10bea-228">若要在增量查询响应中明确哪些更改是由权限更改造成的，可提供 `Prefer: deltashowsharingchanges` 标头。</span><span class="sxs-lookup"><span data-stu-id="10bea-228">To make it clear in the delta query response which changes are the result of permissions being changed, you can provide the `Prefer: deltashowsharingchanges` header.</span></span> <span data-ttu-id="10bea-229">当提供此标头时，由于权限更改而出现在增量查询响应中的所有项目都将具有 `@microsoft.graph.sharedChanged":"True"` OData 注释。</span><span class="sxs-lookup"><span data-stu-id="10bea-229">When this header is provided, all items that appear in the delta query response due to permission changes will have the `@microsoft.graph.sharedChanged":"True"` OData annotation.</span></span> <span data-ttu-id="10bea-230">此功能适用于 SharePoint 和 OneDrive for Business 帐户，但不适用于 OneDrive 消费者版本的帐户。</span><span class="sxs-lookup"><span data-stu-id="10bea-230">This feature is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

> <span data-ttu-id="10bea-231">**注意：** 为了使用 `Prefer: deltashowsharingchanges` 标头，你需要使用 `Prefer: deltashowremovedasdeleted` 和 `Prefer: deltatraversepermissiongaps`。</span><span class="sxs-lookup"><span data-stu-id="10bea-231">**Note:** The use of `Prefer: deltashowsharingchanges` header requires you to use `Prefer: deltashowremovedasdeleted` and `Prefer: deltatraversepermissiongaps`.</span></span> <span data-ttu-id="10bea-232">这些标头值可以在一个标头中连接在一起：`Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`。</span><span class="sxs-lookup"><span data-stu-id="10bea-232">These header values can be joined together in a single header: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.</span></span>

## <a name="error-responses"></a><span data-ttu-id="10bea-233">错误响应</span><span class="sxs-lookup"><span data-stu-id="10bea-233">Error responses</span></span>

<span data-ttu-id="10bea-234">除了上面详述的重新同步错误之外，还请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="10bea-234">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
} -->

