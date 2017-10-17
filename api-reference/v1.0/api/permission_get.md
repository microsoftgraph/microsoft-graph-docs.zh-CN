---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "获取权限"
ms.openlocfilehash: 34171ca2c862857069f904103681ecc9b1646fc7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="d1bc1-102">获取文件或文件夹的共享权限</span><span class="sxs-lookup"><span data-stu-id="d1bc1-102">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="d1bc1-103">返回特定 permission 资源的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-103">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="d1bc1-104">项的有效权限有两个来源：直接对项本身设置权限，或从项上级继承权限。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-104">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="d1bc1-p101">调用方可以检查 `inheritedFrom` 属性来区分是否为继承权限。此属性是引用继承其权限的上级的 [ItemReference](../resources/itemReference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemReference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="d1bc1-107">对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-107">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="d1bc1-108">例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-108">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="d1bc1-109">请参阅 [SharePoint 角色完整列表](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-109">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1bc1-110">权限</span><span class="sxs-lookup"><span data-stu-id="d1bc1-110">Permissions</span></span>

<span data-ttu-id="d1bc1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d1bc1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1bc1-113">Permission type</span></span>      | <span data-ttu-id="d1bc1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1bc1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1bc1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1bc1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d1bc1-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bc1-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1bc1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1bc1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1bc1-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bc1-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1bc1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1bc1-119">Application</span></span> | <span data-ttu-id="d1bc1-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bc1-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1bc1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1bc1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1bc1-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1bc1-122">Optional query parameters</span></span>

<span data-ttu-id="d1bc1-123">此方法支持使用 [$select 查询参数](../../../concepts/query_parameters.md)形成响应。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-123">This method support the [$select query parameter](../../../concepts/query_parameters.md) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="d1bc1-124">响应</span><span class="sxs-lookup"><span data-stu-id="d1bc1-124">Response</span></span>

<span data-ttu-id="d1bc1-125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-125">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1bc1-126">示例</span><span class="sxs-lookup"><span data-stu-id="d1bc1-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1bc1-127">请求</span><span class="sxs-lookup"><span data-stu-id="d1bc1-127">Request</span></span>

<span data-ttu-id="d1bc1-128">下面是请求访问某个文件夹权限的示例。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-128">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="d1bc1-129">响应</span><span class="sxs-lookup"><span data-stu-id="d1bc1-129">Response</span></span>

<span data-ttu-id="d1bc1-130">如果成功，此方法将返回特定 ID 的 [Permission](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-130">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="d1bc1-131">备注</span><span class="sxs-lookup"><span data-stu-id="d1bc1-131">Remarks</span></span>

<span data-ttu-id="d1bc1-132">[权限](../resources/permission.md) 资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-132">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="d1bc1-p104">具有 [**链接**](../resources/sharinglink.md) facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="d1bc1-135">具有 [**invitation**](../resources/sharinginvitation.md) facet 的权限表示通过邀请特定用户或组访问该文件添加的权限。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-135">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

### <a name="error-responses"></a><span data-ttu-id="d1bc1-136">错误响应</span><span class="sxs-lookup"><span data-stu-id="d1bc1-136">Error responses</span></span>

<span data-ttu-id="d1bc1-137">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="d1bc1-137">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
