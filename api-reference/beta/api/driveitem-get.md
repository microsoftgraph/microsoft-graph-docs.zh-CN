---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取文件或文件夹
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 578d7bcbba51876390f9e0134d3c589d64b51e81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454417"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="a530c-102">获取 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="a530c-102">Get a DriveItem resource</span></span>

<span data-ttu-id="a530c-103">通过文件系统路径或 ID 在[驱动器](../resources/drive.md)中检索 [DriveItem](../resources/driveitem.md) 的元数据。</span><span class="sxs-lookup"><span data-stu-id="a530c-103">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a530c-104">权限</span><span class="sxs-lookup"><span data-stu-id="a530c-104">Permissions</span></span>

<span data-ttu-id="a530c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a530c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a530c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a530c-107">Permission type</span></span>      | <span data-ttu-id="a530c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a530c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a530c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a530c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a530c-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a530c-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a530c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a530c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a530c-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a530c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a530c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a530c-113">Application</span></span> | <span data-ttu-id="a530c-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a530c-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a530c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a530c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a530c-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a530c-116">Optional query parameters</span></span>

<span data-ttu-id="a530c-117">此方法支持使用 `$expand` 和 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a530c-117">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="a530c-118">如果某个项具有**子项**关系，在检索该项的元数据时可以使用 [`$expand` 查询字符串参数](/graph/query-parameters) 来包括同一调用中的项的子项。</span><span class="sxs-lookup"><span data-stu-id="a530c-118">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="a530c-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a530c-119">Optional request headers</span></span>

| <span data-ttu-id="a530c-120">名称</span><span class="sxs-lookup"><span data-stu-id="a530c-120">Name</span></span>          | <span data-ttu-id="a530c-121">值</span><span class="sxs-lookup"><span data-stu-id="a530c-121">Value</span></span>  | <span data-ttu-id="a530c-122">说明</span><span class="sxs-lookup"><span data-stu-id="a530c-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a530c-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="a530c-123">if-none-match</span></span> | <span data-ttu-id="a530c-124">String</span><span class="sxs-lookup"><span data-stu-id="a530c-124">String</span></span> | <span data-ttu-id="a530c-125">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="a530c-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="a530c-126">响应</span><span class="sxs-lookup"><span data-stu-id="a530c-126">Response</span></span>

<span data-ttu-id="a530c-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a530c-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a530c-128">示例</span><span class="sxs-lookup"><span data-stu-id="a530c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="a530c-129">请求</span><span class="sxs-lookup"><span data-stu-id="a530c-129">Request</span></span>

<span data-ttu-id="a530c-130">下面是用户的 OneDrive 的根文件夹请求示例。</span><span class="sxs-lookup"><span data-stu-id="a530c-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="a530c-131">响应</span><span class="sxs-lookup"><span data-stu-id="a530c-131">Response</span></span>

<span data-ttu-id="a530c-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a530c-132">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a><span data-ttu-id="a530c-133">备注</span><span class="sxs-lookup"><span data-stu-id="a530c-133">Remarks</span></span>

<span data-ttu-id="a530c-134">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="a530c-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->
