---
author: JeremyKelley
description: 列出 driveItem 上的有效共享权限。
ms.date: 09/10/2017
title: 列出有权访问文件的人
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 346fb5de25021ae9672722a8a128fed224853368
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151473"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="04238-103">列出 driveItem 上的共享权限</span><span class="sxs-lookup"><span data-stu-id="04238-103">List sharing permissions on a driveItem</span></span>

<span data-ttu-id="04238-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04238-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04238-105">列出 [driveItem](../resources/driveitem.md)的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="04238-105">List the effective sharing permissions on a [driveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="04238-106">访问共享权限</span><span class="sxs-lookup"><span data-stu-id="04238-106">Access to sharing permissions</span></span>

<span data-ttu-id="04238-107">权限集合包括潜在的敏感信息，未必适用于所有调用方。</span><span class="sxs-lookup"><span data-stu-id="04238-107">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="04238-108">对于该项目的所有者，将返回所有共享权限。</span><span class="sxs-lookup"><span data-stu-id="04238-108">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="04238-109">这包括共有者。</span><span class="sxs-lookup"><span data-stu-id="04238-109">This includes co-owners.</span></span>
* <span data-ttu-id="04238-110">对于非所有者的调用方，仅返回适用于调用方的共享权限。</span><span class="sxs-lookup"><span data-stu-id="04238-110">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="04238-111">对于能够创建共享权限的调用方，仅返回包含机密信息（例如 `shareId` 和 `webUrl`）的共享权限属性。</span><span class="sxs-lookup"><span data-stu-id="04238-111">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="04238-112">权限</span><span class="sxs-lookup"><span data-stu-id="04238-112">Permissions</span></span>

<span data-ttu-id="04238-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04238-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04238-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="04238-115">Permission type</span></span>      | <span data-ttu-id="04238-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04238-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04238-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04238-117">Delegated (work or school account)</span></span> | <span data-ttu-id="04238-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04238-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="04238-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04238-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04238-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04238-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="04238-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="04238-121">Application</span></span> | <span data-ttu-id="04238-122">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04238-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04238-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04238-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04238-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="04238-124">Optional query parameters</span></span>

<span data-ttu-id="04238-125">此方法支持使用 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="04238-125">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="04238-126">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="04238-126">Optional request headers</span></span>

| <span data-ttu-id="04238-127">名称</span><span class="sxs-lookup"><span data-stu-id="04238-127">Name</span></span>          | <span data-ttu-id="04238-128">类型</span><span class="sxs-lookup"><span data-stu-id="04238-128">Type</span></span>   | <span data-ttu-id="04238-129">说明</span><span class="sxs-lookup"><span data-stu-id="04238-129">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="04238-130">if-none-match</span><span class="sxs-lookup"><span data-stu-id="04238-130">if-none-match</span></span> | <span data-ttu-id="04238-131">string</span><span class="sxs-lookup"><span data-stu-id="04238-131">string</span></span> | <span data-ttu-id="04238-132">如果包含此请求头，且提供的 eTag 与项中的当前 etag 不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="04238-132">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="04238-133">响应</span><span class="sxs-lookup"><span data-stu-id="04238-133">Response</span></span>

<span data-ttu-id="04238-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="04238-134">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="04238-135">DriveItem 的有效共享权限可能有两个来源：</span><span class="sxs-lookup"><span data-stu-id="04238-135">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="04238-136">直接对 DriveItem 本身应用的共享权限</span><span class="sxs-lookup"><span data-stu-id="04238-136">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="04238-137">从 DriveItem 的上级继承的共享权限</span><span class="sxs-lookup"><span data-stu-id="04238-137">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="04238-p103">调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="04238-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="04238-140">示例</span><span class="sxs-lookup"><span data-stu-id="04238-140">Example</span></span>

<span data-ttu-id="04238-141">本示例检索登录用户驱动器中某个项的权限集合。</span><span class="sxs-lookup"><span data-stu-id="04238-141">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>


# <a name="http"></a>[<span data-ttu-id="04238-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="04238-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions
```
# <a name="c"></a>[<span data-ttu-id="04238-143">C#</span><span class="sxs-lookup"><span data-stu-id="04238-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04238-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04238-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04238-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04238-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04238-146">Java</span><span class="sxs-lookup"><span data-stu-id="04238-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04238-147">响应</span><span class="sxs-lookup"><span data-stu-id="04238-147">Response</span></span>

<span data-ttu-id="04238-148">此示例响应包括三个权限，第一个是具有编辑权限的共享链接，第二个是继承自父文件夹且用户名为 John 的显式权限，第三个是由一个应用程序创建的读写共享链接。</span><span class="sxs-lookup"><span data-stu-id="04238-148">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="04238-149">备注</span><span class="sxs-lookup"><span data-stu-id="04238-149">Remarks</span></span>

<span data-ttu-id="04238-p104">不能在 [获取 DriveItem](driveitem-get.md) 的调用过程中或 DriveItem 集合中扩展 DriveItem 的 **权限** 关系。必须直接访问权限属性。</span><span class="sxs-lookup"><span data-stu-id="04238-p104">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="04238-152">错误响应</span><span class="sxs-lookup"><span data-stu-id="04238-152">Error responses</span></span>

<span data-ttu-id="04238-153">请阅读 [错误响应][error-response] 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="04238-153">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
}
-->
