---
title: 添加 noncustodialDataSource
description: 通过发布到 noncustodialSources 集合添加 noncustodialSources。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b6d3dde3e779aad317e3d2827e602d5097300d22
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786788"
---
# <a name="add-noncustodialdatasource"></a><span data-ttu-id="0c34d-103">添加 noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="0c34d-103">Add noncustodialDataSource</span></span>

<span data-ttu-id="0c34d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0c34d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c34d-105">将 noncustodialSources 添加到 [sourceCollection](../api/ediscovery-sourcecollection-get.md)。</span><span class="sxs-lookup"><span data-stu-id="0c34d-105">Add noncustodialSources to a [sourceCollection](../api/ediscovery-sourcecollection-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c34d-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c34d-106">Permissions</span></span>

<span data-ttu-id="0c34d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c34d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c34d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c34d-109">Permission type</span></span>|<span data-ttu-id="0c34d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c34d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c34d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c34d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c34d-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c34d-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0c34d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c34d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c34d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c34d-114">Not supported.</span></span>|
|<span data-ttu-id="0c34d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c34d-115">Application</span></span>|<span data-ttu-id="0c34d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c34d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c34d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c34d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0c34d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c34d-118">Request headers</span></span>

|<span data-ttu-id="0c34d-119">名称</span><span class="sxs-lookup"><span data-stu-id="0c34d-119">Name</span></span>|<span data-ttu-id="0c34d-120">说明</span><span class="sxs-lookup"><span data-stu-id="0c34d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c34d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c34d-121">Authorization</span></span>|<span data-ttu-id="0c34d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c34d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0c34d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c34d-124">Content-Type</span></span>|<span data-ttu-id="0c34d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0c34d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c34d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c34d-127">Request body</span></span>

<span data-ttu-id="0c34d-128">在请求正文中，提供 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c34d-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="0c34d-129">下表显示创建 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c34d-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="0c34d-130">属性</span><span class="sxs-lookup"><span data-stu-id="0c34d-130">Property</span></span>|<span data-ttu-id="0c34d-131">类型</span><span class="sxs-lookup"><span data-stu-id="0c34d-131">Type</span></span>|<span data-ttu-id="0c34d-132">说明</span><span class="sxs-lookup"><span data-stu-id="0c34d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c34d-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="0c34d-133">@odata.id</span></span>|<span data-ttu-id="0c34d-134">String</span><span class="sxs-lookup"><span data-stu-id="0c34d-134">String</span></span>|<span data-ttu-id="0c34d-135">定义空心对象的字符串。</span><span class="sxs-lookup"><span data-stu-id="0c34d-135">String that defines the custodial object.</span></span> <span data-ttu-id="0c34d-136">请参阅下面的示例。</span><span class="sxs-lookup"><span data-stu-id="0c34d-136">See the example that follows.</span></span>  <span data-ttu-id="0c34d-137">@odata.id 可以从 [非custodialDataSource 中检索](../resources/ediscovery-noncustodialdatasource.md)。</span><span class="sxs-lookup"><span data-stu-id="0c34d-137">The @odata.id can be retrieved from the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>|

## <a name="response"></a><span data-ttu-id="0c34d-138">响应</span><span class="sxs-lookup"><span data-stu-id="0c34d-138">Response</span></span>

<span data-ttu-id="0c34d-139">如果成功，此方法在响应正文中返回 响应代码和非 `204 No Content` [custodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c34d-139">If successful, this method returns a `204 No Content` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c34d-140">示例</span><span class="sxs-lookup"><span data-stu-id="0c34d-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c34d-141">请求</span><span class="sxs-lookup"><span data-stu-id="0c34d-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0c34d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c34d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/sourceCollections/12aab1671c834213a84ba219c06f4c5a/noncustodialSources/$ref
Content-Type: application/json
Content-length: 206

{
    "@odata.id": "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
}
```
# <a name="c"></a>[<span data-ttu-id="0c34d-143">C#</span><span class="sxs-lookup"><span data-stu-id="0c34d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-noncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c34d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c34d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-noncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c34d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c34d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-noncustodialdatasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c34d-146">Java</span><span class="sxs-lookup"><span data-stu-id="0c34d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-noncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c34d-147">响应</span><span class="sxs-lookup"><span data-stu-id="0c34d-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
