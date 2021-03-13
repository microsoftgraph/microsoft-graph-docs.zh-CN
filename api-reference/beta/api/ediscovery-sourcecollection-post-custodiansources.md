---
title: 添加 custodianSources
description: 将实际 dataSource 对象添加到源集合。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: aa5f895046548e43b982511be36587e989c38b67
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772574"
---
# <a name="add-custodiansources"></a><span data-ttu-id="8626a-103">添加 custodianSources</span><span class="sxs-lookup"><span data-stu-id="8626a-103">Add custodianSources</span></span>

<span data-ttu-id="8626a-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8626a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8626a-105">将 custodian [dataSource](../resources/ediscovery-datasource.md) 对象添加到源集合。</span><span class="sxs-lookup"><span data-stu-id="8626a-105">Add custodian [dataSource](../resources/ediscovery-datasource.md) objects to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="8626a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8626a-106">Permissions</span></span>

<span data-ttu-id="8626a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8626a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8626a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8626a-109">Permission type</span></span>|<span data-ttu-id="8626a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8626a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8626a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8626a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8626a-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8626a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8626a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8626a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8626a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8626a-114">Not supported.</span></span>|
|<span data-ttu-id="8626a-115">Application</span><span class="sxs-lookup"><span data-stu-id="8626a-115">Application</span></span>|<span data-ttu-id="8626a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8626a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8626a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8626a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8626a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8626a-118">Request headers</span></span>

|<span data-ttu-id="8626a-119">名称</span><span class="sxs-lookup"><span data-stu-id="8626a-119">Name</span></span>|<span data-ttu-id="8626a-120">说明</span><span class="sxs-lookup"><span data-stu-id="8626a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8626a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8626a-121">Authorization</span></span>|<span data-ttu-id="8626a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8626a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8626a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8626a-124">Content-Type</span></span>|<span data-ttu-id="8626a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8626a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8626a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8626a-127">Request body</span></span>

<span data-ttu-id="8626a-128">在请求正文中，提供 [dataSource](../resources/ediscovery-datasource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8626a-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="8626a-129">下表显示创建 [dataSource](../resources/ediscovery-datasource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8626a-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="8626a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8626a-130">Property</span></span>|<span data-ttu-id="8626a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8626a-131">Type</span></span>|<span data-ttu-id="8626a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8626a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8626a-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="8626a-133">@odata.id</span></span>|<span data-ttu-id="8626a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8626a-134">String</span></span>|<span data-ttu-id="8626a-135">定义空心对象的字符串。</span><span class="sxs-lookup"><span data-stu-id="8626a-135">String that defines the custodial object.</span></span> <span data-ttu-id="8626a-136">请参阅下面的示例。</span><span class="sxs-lookup"><span data-stu-id="8626a-136">See the example that follows.</span></span>|

## <a name="response"></a><span data-ttu-id="8626a-137">响应</span><span class="sxs-lookup"><span data-stu-id="8626a-137">Response</span></span>

<span data-ttu-id="8626a-138">如果成功，此方法在响应正文中返回 响应代码和 `204 No Content` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8626a-138">If successful, this method returns a `204 No Content` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8626a-139">示例</span><span class="sxs-lookup"><span data-stu-id="8626a-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8626a-140">请求</span><span class="sxs-lookup"><span data-stu-id="8626a-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8626a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8626a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/custodianSources/$ref
Content-Type: application/json
Content-length: 179

{
  "@odata.id":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
}
```
# <a name="c"></a>[<span data-ttu-id="8626a-142">C#</span><span class="sxs-lookup"><span data-stu-id="8626a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8626a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8626a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8626a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8626a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8626a-145">Java</span><span class="sxs-lookup"><span data-stu-id="8626a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8626a-146">响应</span><span class="sxs-lookup"><span data-stu-id="8626a-146">Response</span></span>

<span data-ttu-id="8626a-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8626a-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```
