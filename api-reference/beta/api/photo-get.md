---
title: 获取照片
description: 检索 photo 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: c1746a347d93dad375635eaf68365af64dfadac9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264482"
---
# <a name="get-photo"></a><span data-ttu-id="e1a8d-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="e1a8d-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1a8d-104">检索 photo 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1a8d-105">权限</span><span class="sxs-lookup"><span data-stu-id="e1a8d-105">Permissions</span></span>
<span data-ttu-id="e1a8d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1a8d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1a8d-108">Permission type</span></span>      | <span data-ttu-id="e1a8d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1a8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1a8d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1a8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1a8d-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e1a8d-111">Files.Read</span></span>    |
|<span data-ttu-id="e1a8d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1a8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a8d-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e1a8d-113">Files.Read</span></span>    |
|<span data-ttu-id="e1a8d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1a8d-114">Application</span></span> | <span data-ttu-id="e1a8d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1a8d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1a8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e1a8d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1a8d-117">Optional query parameters</span></span>
<span data-ttu-id="e1a8d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1a8d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1a8d-119">Request headers</span></span>
| <span data-ttu-id="e1a8d-120">名称</span><span class="sxs-lookup"><span data-stu-id="e1a8d-120">Name</span></span>       | <span data-ttu-id="e1a8d-121">类型</span><span class="sxs-lookup"><span data-stu-id="e1a8d-121">Type</span></span> | <span data-ttu-id="e1a8d-122">说明</span><span class="sxs-lookup"><span data-stu-id="e1a8d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e1a8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1a8d-123">Authorization</span></span>  | <span data-ttu-id="e1a8d-124">string</span><span class="sxs-lookup"><span data-stu-id="e1a8d-124">string</span></span>  | <span data-ttu-id="e1a8d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1a8d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1a8d-127">Request body</span></span>
<span data-ttu-id="e1a8d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1a8d-129">响应</span><span class="sxs-lookup"><span data-stu-id="e1a8d-129">Response</span></span>

<span data-ttu-id="e1a8d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e1a8d-131">示例</span><span class="sxs-lookup"><span data-stu-id="e1a8d-131">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="e1a8d-132">请求</span><span class="sxs-lookup"><span data-stu-id="e1a8d-132">Request</span></span>
<span data-ttu-id="e1a8d-133">下面的示例展示了如何请求获取照片元数据。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="e1a8d-134">响应</span><span class="sxs-lookup"><span data-stu-id="e1a8d-134">Response</span></span>
<span data-ttu-id="e1a8d-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-135">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1a8d-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e1a8d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1a8d-137">C#</span><span class="sxs-lookup"><span data-stu-id="e1a8d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1a8d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1a8d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photo-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1a8d-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="e1a8d-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photo-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="e1a8d-140">请求</span><span class="sxs-lookup"><span data-stu-id="e1a8d-140">Request</span></span>
<span data-ttu-id="e1a8d-141">下面的示例展示了如何请求获取照片字节。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-141">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="e1a8d-142">响应</span><span class="sxs-lookup"><span data-stu-id="e1a8d-142">Response</span></span>
<span data-ttu-id="e1a8d-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e1a8d-143">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
