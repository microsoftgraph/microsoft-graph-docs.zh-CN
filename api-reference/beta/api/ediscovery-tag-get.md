---
title: 获取标记
description: 读取 tag 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c856ccc0c405c50062aaa6befcebc6292a3322e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775278"
---
# <a name="get-tag"></a><span data-ttu-id="e7c95-103">获取标记</span><span class="sxs-lookup"><span data-stu-id="e7c95-103">Get tag</span></span>

<span data-ttu-id="e7c95-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e7c95-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7c95-105">读取 tag [对象的属性和](../resources/ediscovery-tag.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e7c95-105">Read the properties and relationships of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7c95-106">权限</span><span class="sxs-lookup"><span data-stu-id="e7c95-106">Permissions</span></span>

<span data-ttu-id="e7c95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7c95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c95-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7c95-109">Permission type</span></span>|<span data-ttu-id="e7c95-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7c95-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c95-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7c95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c95-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c95-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e7c95-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7c95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c95-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7c95-114">Not supported.</span></span>|
|<span data-ttu-id="e7c95-115">Application</span><span class="sxs-lookup"><span data-stu-id="e7c95-115">Application</span></span>|<span data-ttu-id="e7c95-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7c95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c95-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7c95-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7c95-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e7c95-118">Optional query parameters</span></span>

<span data-ttu-id="e7c95-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e7c95-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e7c95-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e7c95-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7c95-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7c95-121">Request headers</span></span>

|<span data-ttu-id="e7c95-122">名称</span><span class="sxs-lookup"><span data-stu-id="e7c95-122">Name</span></span>|<span data-ttu-id="e7c95-123">说明</span><span class="sxs-lookup"><span data-stu-id="e7c95-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e7c95-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c95-124">Authorization</span></span>|<span data-ttu-id="e7c95-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7c95-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c95-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7c95-127">Request body</span></span>

<span data-ttu-id="e7c95-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e7c95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7c95-129">响应</span><span class="sxs-lookup"><span data-stu-id="e7c95-129">Response</span></span>

<span data-ttu-id="e7c95-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7c95-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7c95-131">示例</span><span class="sxs-lookup"><span data-stu-id="e7c95-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7c95-132">请求</span><span class="sxs-lookup"><span data-stu-id="e7c95-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e7c95-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7c95-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
```
# <a name="c"></a>[<span data-ttu-id="e7c95-134">C#</span><span class="sxs-lookup"><span data-stu-id="e7c95-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7c95-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7c95-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7c95-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7c95-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7c95-137">Java</span><span class="sxs-lookup"><span data-stu-id="e7c95-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e7c95-138">响应</span><span class="sxs-lookup"><span data-stu-id="e7c95-138">Response</span></span>

<span data-ttu-id="e7c95-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e7c95-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/tags/$entity",
    "displayName": "Responsiveness",
    "description": "Indicates the responsiveness of the document",
    "lastModifiedDateTime": "2021-01-11T19:32:23.1903658Z",
    "childSelectability": "One",
    "id": "e54b3f535b434a9a8743b84e34c00504",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalName": "admin@contoso.com"
        }
    },
    "childTags": []
}
```
