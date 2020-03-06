---
title: 获取照片
description: 检索 photo 对象的属性和关系。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8f2aac2615c570e245b39b37006e12743c48da6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511024"
---
# <a name="get-photo"></a><span data-ttu-id="767df-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="767df-103">Get photo</span></span>

<span data-ttu-id="767df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="767df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="767df-105">检索 photo 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="767df-105">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="767df-106">权限</span><span class="sxs-lookup"><span data-stu-id="767df-106">Permissions</span></span>
<span data-ttu-id="767df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="767df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="767df-109">Permission type</span></span>      | <span data-ttu-id="767df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="767df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="767df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="767df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="767df-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="767df-112">Files.Read</span></span>    |
|<span data-ttu-id="767df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="767df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="767df-114">Files.Read</span><span class="sxs-lookup"><span data-stu-id="767df-114">Files.Read</span></span>    |
|<span data-ttu-id="767df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="767df-115">Application</span></span> | <span data-ttu-id="767df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="767df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="767df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="767df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="767df-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="767df-118">Optional query parameters</span></span>
<span data-ttu-id="767df-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="767df-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="767df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="767df-120">Request headers</span></span>
| <span data-ttu-id="767df-121">名称</span><span class="sxs-lookup"><span data-stu-id="767df-121">Name</span></span>       | <span data-ttu-id="767df-122">类型</span><span class="sxs-lookup"><span data-stu-id="767df-122">Type</span></span> | <span data-ttu-id="767df-123">说明</span><span class="sxs-lookup"><span data-stu-id="767df-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="767df-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="767df-124">Authorization</span></span>  | <span data-ttu-id="767df-125">string</span><span class="sxs-lookup"><span data-stu-id="767df-125">string</span></span>  | <span data-ttu-id="767df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="767df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="767df-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="767df-128">Request body</span></span>
<span data-ttu-id="767df-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="767df-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="767df-130">响应</span><span class="sxs-lookup"><span data-stu-id="767df-130">Response</span></span>

<span data-ttu-id="767df-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="767df-131">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="767df-132">示例</span><span class="sxs-lookup"><span data-stu-id="767df-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="767df-133">请求</span><span class="sxs-lookup"><span data-stu-id="767df-133">Request</span></span>
<span data-ttu-id="767df-134">下面的示例展示了如何请求获取照片元数据。</span><span class="sxs-lookup"><span data-stu-id="767df-134">Here is an example of the request for photo metadata.</span></span>

# <a name="http"></a>[<span data-ttu-id="767df-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="767df-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="767df-136">C#</span><span class="sxs-lookup"><span data-stu-id="767df-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="767df-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="767df-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="767df-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="767df-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="767df-139">Java</span><span class="sxs-lookup"><span data-stu-id="767df-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="767df-140">响应</span><span class="sxs-lookup"><span data-stu-id="767df-140">Response</span></span>
<span data-ttu-id="767df-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="767df-141">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="767df-142">请求</span><span class="sxs-lookup"><span data-stu-id="767df-142">Request</span></span>
<span data-ttu-id="767df-143">下面的示例展示了如何请求获取照片字节。</span><span class="sxs-lookup"><span data-stu-id="767df-143">Here is an example of the request for the photo bytes.</span></span>

# <a name="http"></a>[<span data-ttu-id="767df-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="767df-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
# <a name="c"></a>[<span data-ttu-id="767df-145">C#</span><span class="sxs-lookup"><span data-stu-id="767df-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="767df-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="767df-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="767df-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="767df-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="767df-148">Java</span><span class="sxs-lookup"><span data-stu-id="767df-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="767df-149">响应</span><span class="sxs-lookup"><span data-stu-id="767df-149">Response</span></span>
<span data-ttu-id="767df-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="767df-150">Here is an example of the response.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
