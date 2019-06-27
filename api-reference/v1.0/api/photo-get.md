---
title: 获取照片
description: 检索 photo 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 513382d58690fdb2198e4974030cd1d9cafd65c7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274233"
---
# <a name="get-photo"></a><span data-ttu-id="7d5f8-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="7d5f8-103">Get photo</span></span>

<span data-ttu-id="7d5f8-104">检索 photo 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d5f8-105">权限</span><span class="sxs-lookup"><span data-stu-id="7d5f8-105">Permissions</span></span>
<span data-ttu-id="7d5f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d5f8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d5f8-108">Permission type</span></span>      | <span data-ttu-id="7d5f8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d5f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d5f8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d5f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d5f8-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="7d5f8-111">Files.Read</span></span>    |
|<span data-ttu-id="7d5f8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d5f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d5f8-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="7d5f8-113">Files.Read</span></span>    |
|<span data-ttu-id="7d5f8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d5f8-114">Application</span></span> | <span data-ttu-id="7d5f8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d5f8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d5f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d5f8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7d5f8-117">Optional query parameters</span></span>
<span data-ttu-id="7d5f8-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d5f8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d5f8-119">Request headers</span></span>
| <span data-ttu-id="7d5f8-120">名称</span><span class="sxs-lookup"><span data-stu-id="7d5f8-120">Name</span></span>       | <span data-ttu-id="7d5f8-121">类型</span><span class="sxs-lookup"><span data-stu-id="7d5f8-121">Type</span></span> | <span data-ttu-id="7d5f8-122">说明</span><span class="sxs-lookup"><span data-stu-id="7d5f8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7d5f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d5f8-123">Authorization</span></span>  | <span data-ttu-id="7d5f8-124">string</span><span class="sxs-lookup"><span data-stu-id="7d5f8-124">string</span></span>  | <span data-ttu-id="7d5f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d5f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d5f8-127">Request body</span></span>
<span data-ttu-id="7d5f8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d5f8-129">响应</span><span class="sxs-lookup"><span data-stu-id="7d5f8-129">Response</span></span>

<span data-ttu-id="7d5f8-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d5f8-131">示例</span><span class="sxs-lookup"><span data-stu-id="7d5f8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d5f8-132">请求</span><span class="sxs-lookup"><span data-stu-id="7d5f8-132">Request</span></span>
<span data-ttu-id="7d5f8-133">下面的示例展示了如何请求获取照片元数据。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="7d5f8-134">响应</span><span class="sxs-lookup"><span data-stu-id="7d5f8-134">Response</span></span>
<span data-ttu-id="7d5f8-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-135">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7d5f8-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7d5f8-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7d5f8-137">C#</span><span class="sxs-lookup"><span data-stu-id="7d5f8-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d5f8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d5f8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photo-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7d5f8-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="7d5f8-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photo-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="7d5f8-140">请求</span><span class="sxs-lookup"><span data-stu-id="7d5f8-140">Request</span></span>
<span data-ttu-id="7d5f8-141">下面的示例展示了如何请求获取照片字节。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-141">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="7d5f8-142">响应</span><span class="sxs-lookup"><span data-stu-id="7d5f8-142">Response</span></span>
<span data-ttu-id="7d5f8-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7d5f8-143">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Edm.Stream" } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7d5f8-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7d5f8-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7d5f8-145">C#</span><span class="sxs-lookup"><span data-stu-id="7d5f8-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photo_value-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d5f8-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d5f8-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photo_value-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7d5f8-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="7d5f8-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photo_value-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
