---
title: 列出 sourceCollections
description: 从 case 对象获取 sourceCollections 资源的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 801a526ef92cdffb5e262a830b5708db3a11e0ca
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080294"
---
# <a name="list-sourcecollections"></a><span data-ttu-id="d963f-103">列出 sourceCollections</span><span class="sxs-lookup"><span data-stu-id="d963f-103">List sourceCollections</span></span>

<span data-ttu-id="d963f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d963f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d963f-105">从 case 对象获取[sourceCollections](../resources/ediscovery-sourcecollection.md)[列表。](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="d963f-105">Get the list of [sourceCollections](../resources/ediscovery-sourcecollection.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d963f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d963f-106">Permissions</span></span>

<span data-ttu-id="d963f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d963f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d963f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d963f-109">Permission type</span></span>|<span data-ttu-id="d963f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d963f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d963f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d963f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d963f-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d963f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d963f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d963f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d963f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d963f-114">Not supported.</span></span>|
|<span data-ttu-id="d963f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d963f-115">Application</span></span>|<span data-ttu-id="d963f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d963f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d963f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d963f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d963f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d963f-118">Optional query parameters</span></span>

<span data-ttu-id="d963f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d963f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d963f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d963f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d963f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d963f-121">Request headers</span></span>

|<span data-ttu-id="d963f-122">名称</span><span class="sxs-lookup"><span data-stu-id="d963f-122">Name</span></span>|<span data-ttu-id="d963f-123">说明</span><span class="sxs-lookup"><span data-stu-id="d963f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d963f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d963f-124">Authorization</span></span>|<span data-ttu-id="d963f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d963f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d963f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d963f-127">Request body</span></span>

<span data-ttu-id="d963f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d963f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d963f-129">响应</span><span class="sxs-lookup"><span data-stu-id="d963f-129">Response</span></span>

<span data-ttu-id="d963f-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d963f-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d963f-131">示例</span><span class="sxs-lookup"><span data-stu-id="d963f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d963f-132">请求</span><span class="sxs-lookup"><span data-stu-id="d963f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d963f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d963f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections
```
# <a name="c"></a>[<span data-ttu-id="d963f-134">C#</span><span class="sxs-lookup"><span data-stu-id="d963f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d963f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d963f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d963f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d963f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d963f-137">Java</span><span class="sxs-lookup"><span data-stu-id="d963f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d963f-138">响应</span><span class="sxs-lookup"><span data-stu-id="d963f-138">Response</span></span>

> <span data-ttu-id="d963f-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d963f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.sourceCollection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/sourceCollections",
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2020-12-31T18:54:28.80694Z",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "contentQuery": "subject:'Quarterly Financials'",
            "dataSourceScopes": "allTenantMailboxes",
            "id": "fe5ef84e9c8c45819c056f6eb261718e",
            "displayName": "Quarterly Financials",
            "createdDateTime": "2020-12-11T22:56:14.2329133Z"
        }
    ]
}
```
