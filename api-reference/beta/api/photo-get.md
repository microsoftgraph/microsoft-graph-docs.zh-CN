---
title: 获取照片
description: 检索 photo 对象的属性和关系。
ms.openlocfilehash: 16e0849d3cc1a9a98226b6f34221a8a37cec72b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041464"
---
# <a name="get-photo"></a><span data-ttu-id="865f1-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="865f1-103">Get photo</span></span>

> <span data-ttu-id="865f1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="865f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="865f1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="865f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="865f1-106">检索 photo 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="865f1-106">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="865f1-107">权限</span><span class="sxs-lookup"><span data-stu-id="865f1-107">Permissions</span></span>
<span data-ttu-id="865f1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="865f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="865f1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="865f1-110">Permission type</span></span>      | <span data-ttu-id="865f1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="865f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="865f1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="865f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="865f1-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="865f1-113">Files.Read</span></span>    |
|<span data-ttu-id="865f1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="865f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="865f1-115">Files.Read</span><span class="sxs-lookup"><span data-stu-id="865f1-115">Files.Read</span></span>    |
|<span data-ttu-id="865f1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="865f1-116">Application</span></span> | <span data-ttu-id="865f1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="865f1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="865f1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="865f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="865f1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="865f1-119">Optional query parameters</span></span>
<span data-ttu-id="865f1-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="865f1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="865f1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="865f1-121">Request headers</span></span>
| <span data-ttu-id="865f1-122">名称</span><span class="sxs-lookup"><span data-stu-id="865f1-122">Name</span></span>       | <span data-ttu-id="865f1-123">类型</span><span class="sxs-lookup"><span data-stu-id="865f1-123">Type</span></span> | <span data-ttu-id="865f1-124">说明</span><span class="sxs-lookup"><span data-stu-id="865f1-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="865f1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="865f1-125">Authorization</span></span>  | <span data-ttu-id="865f1-126">string</span><span class="sxs-lookup"><span data-stu-id="865f1-126">string</span></span>  | <span data-ttu-id="865f1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="865f1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="865f1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="865f1-129">Request body</span></span>
<span data-ttu-id="865f1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="865f1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="865f1-131">响应</span><span class="sxs-lookup"><span data-stu-id="865f1-131">Response</span></span>

<span data-ttu-id="865f1-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="865f1-132">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="865f1-133">示例</span><span class="sxs-lookup"><span data-stu-id="865f1-133">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="865f1-134">请求</span><span class="sxs-lookup"><span data-stu-id="865f1-134">Request</span></span>
<span data-ttu-id="865f1-135">下面的示例展示了如何请求获取照片元数据。</span><span class="sxs-lookup"><span data-stu-id="865f1-135">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="865f1-136">响应</span><span class="sxs-lookup"><span data-stu-id="865f1-136">Response</span></span>
<span data-ttu-id="865f1-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="865f1-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="request"></a><span data-ttu-id="865f1-138">请求</span><span class="sxs-lookup"><span data-stu-id="865f1-138">Request</span></span>
<span data-ttu-id="865f1-139">下面的示例展示了如何请求获取照片字节。</span><span class="sxs-lookup"><span data-stu-id="865f1-139">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="865f1-140">响应</span><span class="sxs-lookup"><span data-stu-id="865f1-140">Response</span></span>
<span data-ttu-id="865f1-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="865f1-141">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored","@odata.type": "stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
