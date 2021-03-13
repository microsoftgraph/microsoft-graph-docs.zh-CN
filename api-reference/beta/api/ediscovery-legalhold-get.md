---
title: 获取 legalHold
description: 读取 legalHold 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5fadb4d34afe3f7f6642d0b72f9a33754355b8a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773107"
---
# <a name="get-legalhold"></a><span data-ttu-id="942bf-103">获取 legalHold</span><span class="sxs-lookup"><span data-stu-id="942bf-103">Get legalHold</span></span>

<span data-ttu-id="942bf-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="942bf-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942bf-105">读取 [legalHold 对象的属性和](../resources/ediscovery-legalhold.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="942bf-105">Read the properties and relationships of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="942bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="942bf-106">Permissions</span></span>

<span data-ttu-id="942bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="942bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="942bf-109">Permission type</span></span>|<span data-ttu-id="942bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="942bf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="942bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="942bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="942bf-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942bf-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="942bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="942bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="942bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="942bf-114">Not supported.</span></span>|
|<span data-ttu-id="942bf-115">Application</span><span class="sxs-lookup"><span data-stu-id="942bf-115">Application</span></span>|<span data-ttu-id="942bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="942bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="942bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="942bf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="942bf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="942bf-118">Optional query parameters</span></span>

<span data-ttu-id="942bf-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="942bf-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="942bf-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="942bf-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="942bf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="942bf-121">Request headers</span></span>

|<span data-ttu-id="942bf-122">名称</span><span class="sxs-lookup"><span data-stu-id="942bf-122">Name</span></span>|<span data-ttu-id="942bf-123">说明</span><span class="sxs-lookup"><span data-stu-id="942bf-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="942bf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="942bf-124">Authorization</span></span>|<span data-ttu-id="942bf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="942bf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="942bf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="942bf-127">Request body</span></span>

<span data-ttu-id="942bf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="942bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="942bf-129">响应</span><span class="sxs-lookup"><span data-stu-id="942bf-129">Response</span></span>

<span data-ttu-id="942bf-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="942bf-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="942bf-131">示例</span><span class="sxs-lookup"><span data-stu-id="942bf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="942bf-132">请求</span><span class="sxs-lookup"><span data-stu-id="942bf-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="942bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="942bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```
# <a name="c"></a>[<span data-ttu-id="942bf-134">C#</span><span class="sxs-lookup"><span data-stu-id="942bf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-legalhold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="942bf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="942bf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-legalhold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="942bf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="942bf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-legalhold-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="942bf-137">Java</span><span class="sxs-lookup"><span data-stu-id="942bf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-legalhold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="942bf-138">响应</span><span class="sxs-lookup"><span data-stu-id="942bf-138">Response</span></span>

<span data-ttu-id="942bf-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="942bf-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.ediscovery.legalHold",
    "id": "700cd868-d868-700c-68d8-0c7068d80c70",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "isEnabled": "Boolean",
    "status": "String",
    "contentQuery": "String",
    "errors": [
      "String"
    ],
    "displayName": "String",
    "createdDateTime": "String (timestamp)"
  }
}
```
