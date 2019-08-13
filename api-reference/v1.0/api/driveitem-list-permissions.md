---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出有权访问文件的权限
localization_priority: Normal
ms.prod: sharepoint
description: 列出 DriveItem 中的有效共享权限。
doc_type: apiPageType
ms.openlocfilehash: 19fa8efb45570622b969fba060cd8d3da360166c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376050"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="f6cb2-103">列出 DriveItem 中的共享权限</span><span class="sxs-lookup"><span data-stu-id="f6cb2-103">List sharing permissions on a DriveItem</span></span>

<span data-ttu-id="f6cb2-104">列出 [DriveItem](../resources/driveitem.md) 中的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-104">List the effective sharing permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="f6cb2-105">访问共享权限</span><span class="sxs-lookup"><span data-stu-id="f6cb2-105">Access to sharing permissions</span></span>

<span data-ttu-id="f6cb2-106">权限集合包括潜在的敏感信息，不可能适用于每个调用方。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="f6cb2-107">对于该项目的所有者，将返回所有共享权限。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-107">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="f6cb2-108">这包括共有者。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-108">This includes co-owners.</span></span>
* <span data-ttu-id="f6cb2-109">对于非所有者的调用方，仅返回应用于调用方的共享权限。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-109">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="f6cb2-110">对于能够创建共享权限的调用方，仅返回包含机密信息（例如 `shareId` 和 `webUrl`）的共享权限属性。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-110">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6cb2-111">权限</span><span class="sxs-lookup"><span data-stu-id="f6cb2-111">Permissions</span></span>

<span data-ttu-id="f6cb2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6cb2-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6cb2-114">Permission type</span></span>      | <span data-ttu-id="f6cb2-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6cb2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6cb2-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6cb2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f6cb2-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6cb2-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6cb2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6cb2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6cb2-119">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6cb2-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6cb2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6cb2-120">Application</span></span> | <span data-ttu-id="f6cb2-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6cb2-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6cb2-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6cb2-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6cb2-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f6cb2-123">Optional query parameters</span></span>

<span data-ttu-id="f6cb2-124">此方法支持使用 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-124">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="f6cb2-125">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f6cb2-125">Optional request headers</span></span>

| <span data-ttu-id="f6cb2-126">名称</span><span class="sxs-lookup"><span data-stu-id="f6cb2-126">Name</span></span>          | <span data-ttu-id="f6cb2-127">类型</span><span class="sxs-lookup"><span data-stu-id="f6cb2-127">Type</span></span>   | <span data-ttu-id="f6cb2-128">说明</span><span class="sxs-lookup"><span data-stu-id="f6cb2-128">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f6cb2-129">if-none-match</span><span class="sxs-lookup"><span data-stu-id="f6cb2-129">if-none-match</span></span> | <span data-ttu-id="f6cb2-130">string</span><span class="sxs-lookup"><span data-stu-id="f6cb2-130">string</span></span> | <span data-ttu-id="f6cb2-131">如果包含此请求头，且提供的 eTag 与项中的当前 etag 不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-131">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="f6cb2-132">响应</span><span class="sxs-lookup"><span data-stu-id="f6cb2-132">Response</span></span>

<span data-ttu-id="f6cb2-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Permission](../resources/permission.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-133">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="f6cb2-134">DriveItem 的有效共享权限可能有两个来源：</span><span class="sxs-lookup"><span data-stu-id="f6cb2-134">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="f6cb2-135">直接对 DriveItem 本身应用的共享权限</span><span class="sxs-lookup"><span data-stu-id="f6cb2-135">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="f6cb2-136">从 DriveItem 的上级继承的共享权限</span><span class="sxs-lookup"><span data-stu-id="f6cb2-136">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="f6cb2-p103">调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="f6cb2-p104">对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。 例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。 请参阅 [SharePoint 角色完整列表](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="f6cb2-142">示例</span><span class="sxs-lookup"><span data-stu-id="f6cb2-142">Example</span></span>

<span data-ttu-id="f6cb2-143">本示例检索登录用户驱动器中某个项的权限集合。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-143">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f6cb2-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f6cb2-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6cb2-145">C#</span><span class="sxs-lookup"><span data-stu-id="f6cb2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6cb2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6cb2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6cb2-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="f6cb2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f6cb2-148">Java</span><span class="sxs-lookup"><span data-stu-id="f6cb2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6cb2-149">响应</span><span class="sxs-lookup"><span data-stu-id="f6cb2-149">Response</span></span>

<span data-ttu-id="f6cb2-150">此示例响应包括三个权限，第一个是具有编辑权限的共享链接，第二个是继承自父文件夹用户名为 John 的显式权限，第三个是由一个应用程序创建的读写共享链接。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-150">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="f6cb2-151">注解</span><span class="sxs-lookup"><span data-stu-id="f6cb2-151">Remarks</span></span>

<span data-ttu-id="f6cb2-p105">不能在 [获取 DriveItem](driveitem-get.md) 的调用过程中或 DriveItem 集合中扩展 DriveItem 的**权限**关系。必须直接访问权限属性。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="f6cb2-154">错误响应</span><span class="sxs-lookup"><span data-stu-id="f6cb2-154">Error responses</span></span>

<span data-ttu-id="f6cb2-155">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="f6cb2-155">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
} -->
