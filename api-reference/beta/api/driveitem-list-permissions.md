---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出有权访问文件的权限
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b3d096b42b06226580bf7d7b430351ab5719ad4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589146"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="a29f0-102">列出 DriveItem 中的共享权限</span><span class="sxs-lookup"><span data-stu-id="a29f0-102">List sharing permissions on a DriveItem</span></span>

<span data-ttu-id="a29f0-103">列出 [DriveItem](../resources/driveitem.md) 中的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="a29f0-103">List the effective sharing permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="a29f0-104">访问共享权限</span><span class="sxs-lookup"><span data-stu-id="a29f0-104">Access to sharing permissions</span></span>

<span data-ttu-id="a29f0-105">权限集合包括潜在的敏感信息，不可能适用于每个调用方。</span><span class="sxs-lookup"><span data-stu-id="a29f0-105">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="a29f0-106">对于该项目的所有者，将返回所有共享权限。</span><span class="sxs-lookup"><span data-stu-id="a29f0-106">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="a29f0-107">这包括共有者。</span><span class="sxs-lookup"><span data-stu-id="a29f0-107">This includes co-owners.</span></span>
* <span data-ttu-id="a29f0-108">对于非所有者的调用方，仅返回应用于调用方的共享权限。</span><span class="sxs-lookup"><span data-stu-id="a29f0-108">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="a29f0-109">对于能够创建共享权限的调用方，仅返回包含机密信息（例如 `shareId` 和 `webUrl`）的共享权限属性。</span><span class="sxs-lookup"><span data-stu-id="a29f0-109">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="a29f0-110">权限</span><span class="sxs-lookup"><span data-stu-id="a29f0-110">Permissions</span></span>

<span data-ttu-id="a29f0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a29f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a29f0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a29f0-113">Permission type</span></span>      | <span data-ttu-id="a29f0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a29f0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a29f0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a29f0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a29f0-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a29f0-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a29f0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a29f0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a29f0-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a29f0-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a29f0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a29f0-119">Application</span></span> | <span data-ttu-id="a29f0-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a29f0-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a29f0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a29f0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a29f0-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a29f0-122">Optional query parameters</span></span>

<span data-ttu-id="a29f0-123">此方法支持使用 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a29f0-123">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="a29f0-124">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a29f0-124">Optional request headers</span></span>

| <span data-ttu-id="a29f0-125">名称</span><span class="sxs-lookup"><span data-stu-id="a29f0-125">Name</span></span>          | <span data-ttu-id="a29f0-126">类型</span><span class="sxs-lookup"><span data-stu-id="a29f0-126">Type</span></span>   | <span data-ttu-id="a29f0-127">说明</span><span class="sxs-lookup"><span data-stu-id="a29f0-127">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a29f0-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="a29f0-128">if-none-match</span></span> | <span data-ttu-id="a29f0-129">string</span><span class="sxs-lookup"><span data-stu-id="a29f0-129">string</span></span> | <span data-ttu-id="a29f0-130">如果包含此请求头，且提供的 eTag 与项中的当前 etag 不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="a29f0-130">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="a29f0-131">响应</span><span class="sxs-lookup"><span data-stu-id="a29f0-131">Response</span></span>

<span data-ttu-id="a29f0-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Permission](../resources/permission.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="a29f0-132">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="a29f0-133">DriveItem 的有效共享权限可能有两个来源：</span><span class="sxs-lookup"><span data-stu-id="a29f0-133">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="a29f0-134">直接对 DriveItem 本身应用的共享权限</span><span class="sxs-lookup"><span data-stu-id="a29f0-134">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="a29f0-135">从 DriveItem 的上级继承的共享权限</span><span class="sxs-lookup"><span data-stu-id="a29f0-135">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="a29f0-p103">调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a29f0-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="a29f0-p104">对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。 例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。 请参阅 [SharePoint 角色完整列表](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)。</span><span class="sxs-lookup"><span data-stu-id="a29f0-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="a29f0-141">示例</span><span class="sxs-lookup"><span data-stu-id="a29f0-141">Example</span></span>

<span data-ttu-id="a29f0-142">本示例检索登录用户驱动器中某个项的权限集合。</span><span class="sxs-lookup"><span data-stu-id="a29f0-142">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a><span data-ttu-id="a29f0-143">响应</span><span class="sxs-lookup"><span data-stu-id="a29f0-143">Response</span></span>

<span data-ttu-id="a29f0-144">此示例响应包括三个权限，第一个是具有编辑权限的共享链接，第二个是继承自父文件夹用户名为 John 的显式权限，第三个是由一个应用程序创建的读写共享链接。</span><span class="sxs-lookup"><span data-stu-id="a29f0-144">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a29f0-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a29f0-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a29f0-146">语言</span><span class="sxs-lookup"><span data-stu-id="a29f0-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-item-permissions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a29f0-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="a29f0-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-item-permissions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="a29f0-148">注解</span><span class="sxs-lookup"><span data-stu-id="a29f0-148">Remarks</span></span>

<span data-ttu-id="a29f0-p105">不能在 [获取 DriveItem](driveitem-get.md) 的调用过程中或 DriveItem 集合中扩展 DriveItem 的**权限**关系。必须直接访问权限属性。</span><span class="sxs-lookup"><span data-stu-id="a29f0-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="a29f0-151">错误响应</span><span class="sxs-lookup"><span data-stu-id="a29f0-151">Error responses</span></span>

<span data-ttu-id="a29f0-152">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="a29f0-152">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-list-permissions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-list-permissions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
