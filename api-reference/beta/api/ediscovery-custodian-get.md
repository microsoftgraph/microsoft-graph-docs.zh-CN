---
title: 获取保管人
description: 读取保管人对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 18fc6d6bb852b8615c3b30e34bd88789c026390d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946314"
---
# <a name="get-custodian"></a><span data-ttu-id="e9a97-103">获取保管人</span><span class="sxs-lookup"><span data-stu-id="e9a97-103">Get custodian</span></span>

<span data-ttu-id="e9a97-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e9a97-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a97-105">读取保管人对象 [的属性](../resources/ediscovery-custodian.md) 和关系。</span><span class="sxs-lookup"><span data-stu-id="e9a97-105">Read the properties and relationships of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9a97-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9a97-106">Permissions</span></span>

<span data-ttu-id="e9a97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9a97-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9a97-109">Permission type</span></span>|<span data-ttu-id="e9a97-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9a97-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9a97-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9a97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9a97-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9a97-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e9a97-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9a97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9a97-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9a97-114">Not supported.</span></span>|
|<span data-ttu-id="e9a97-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9a97-115">Application</span></span>|<span data-ttu-id="e9a97-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9a97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9a97-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9a97-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caesId}/custodians/{custodianId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9a97-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9a97-118">Optional query parameters</span></span>

<span data-ttu-id="e9a97-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9a97-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e9a97-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e9a97-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9a97-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9a97-121">Request headers</span></span>

|<span data-ttu-id="e9a97-122">名称</span><span class="sxs-lookup"><span data-stu-id="e9a97-122">Name</span></span>|<span data-ttu-id="e9a97-123">说明</span><span class="sxs-lookup"><span data-stu-id="e9a97-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e9a97-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9a97-124">Authorization</span></span>|<span data-ttu-id="e9a97-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9a97-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9a97-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9a97-127">Request body</span></span>

<span data-ttu-id="e9a97-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9a97-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9a97-129">响应</span><span class="sxs-lookup"><span data-stu-id="e9a97-129">Response</span></span>

<span data-ttu-id="e9a97-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9a97-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9a97-131">示例</span><span class="sxs-lookup"><span data-stu-id="e9a97-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9a97-132">请求</span><span class="sxs-lookup"><span data-stu-id="e9a97-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e9a97-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a97-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
```
# <a name="c"></a>[<span data-ttu-id="e9a97-134">C#</span><span class="sxs-lookup"><span data-stu-id="e9a97-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9a97-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9a97-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9a97-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9a97-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9a97-137">Java</span><span class="sxs-lookup"><span data-stu-id="e9a97-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9a97-138">响应</span><span class="sxs-lookup"><span data-stu-id="e9a97-138">Response</span></span>

<span data-ttu-id="e9a97-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9a97-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": true,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T20:59:55.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
