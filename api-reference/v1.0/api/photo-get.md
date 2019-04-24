---
title: 获取照片
description: 检索 photo 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 808eda22550eb6c9affed42bdac9a21189a22cf0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521101"
---
# <a name="get-photo"></a><span data-ttu-id="3feba-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="3feba-103">Get photo</span></span>

<span data-ttu-id="3feba-104">检索 photo 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3feba-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3feba-105">权限</span><span class="sxs-lookup"><span data-stu-id="3feba-105">Permissions</span></span>
<span data-ttu-id="3feba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3feba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3feba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3feba-108">Permission type</span></span>      | <span data-ttu-id="3feba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3feba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3feba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3feba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3feba-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="3feba-111">Files.Read</span></span>    |
|<span data-ttu-id="3feba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3feba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3feba-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="3feba-113">Files.Read</span></span>    |
|<span data-ttu-id="3feba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3feba-114">Application</span></span> | <span data-ttu-id="3feba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3feba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3feba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3feba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3feba-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3feba-117">Optional query parameters</span></span>
<span data-ttu-id="3feba-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3feba-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3feba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3feba-119">Request headers</span></span>
| <span data-ttu-id="3feba-120">名称</span><span class="sxs-lookup"><span data-stu-id="3feba-120">Name</span></span>       | <span data-ttu-id="3feba-121">类型</span><span class="sxs-lookup"><span data-stu-id="3feba-121">Type</span></span> | <span data-ttu-id="3feba-122">说明</span><span class="sxs-lookup"><span data-stu-id="3feba-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3feba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3feba-123">Authorization</span></span>  | <span data-ttu-id="3feba-124">string</span><span class="sxs-lookup"><span data-stu-id="3feba-124">string</span></span>  | <span data-ttu-id="3feba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3feba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3feba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3feba-127">Request body</span></span>
<span data-ttu-id="3feba-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3feba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3feba-129">响应</span><span class="sxs-lookup"><span data-stu-id="3feba-129">Response</span></span>

<span data-ttu-id="3feba-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3feba-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3feba-131">示例</span><span class="sxs-lookup"><span data-stu-id="3feba-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3feba-132">请求</span><span class="sxs-lookup"><span data-stu-id="3feba-132">Request</span></span>
<span data-ttu-id="3feba-133">下面的示例展示了如何请求获取照片元数据。</span><span class="sxs-lookup"><span data-stu-id="3feba-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="3feba-134">响应</span><span class="sxs-lookup"><span data-stu-id="3feba-134">Response</span></span>
<span data-ttu-id="3feba-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3feba-135">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="3feba-136">请求</span><span class="sxs-lookup"><span data-stu-id="3feba-136">Request</span></span>
<span data-ttu-id="3feba-137">下面的示例展示了如何请求获取照片字节。</span><span class="sxs-lookup"><span data-stu-id="3feba-137">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="3feba-138">响应</span><span class="sxs-lookup"><span data-stu-id="3feba-138">Response</span></span>
<span data-ttu-id="3feba-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3feba-139">Here is an example of the response.</span></span>

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
  "tocPath": ""
}-->
