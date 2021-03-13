---
title: 更新保管人
description: 更新保管人对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 82a5a1c401c3d9c1fdcd90d7d0f5bdda10d68982
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773184"
---
# <a name="update-custodian"></a><span data-ttu-id="bb0a7-103">更新保管人</span><span class="sxs-lookup"><span data-stu-id="bb0a7-103">Update custodian</span></span>

<span data-ttu-id="bb0a7-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bb0a7-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb0a7-105">更新保管 [人对象](../resources/ediscovery-custodian.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-105">Update the properties of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb0a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb0a7-106">Permissions</span></span>

<span data-ttu-id="bb0a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb0a7-109">Permission type</span></span>|<span data-ttu-id="bb0a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb0a7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb0a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb0a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb0a7-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb0a7-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bb0a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb0a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb0a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-114">Not supported.</span></span>|
|<span data-ttu-id="bb0a7-115">Application</span><span class="sxs-lookup"><span data-stu-id="bb0a7-115">Application</span></span>|<span data-ttu-id="bb0a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb0a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb0a7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="bb0a7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb0a7-118">Request headers</span></span>

|<span data-ttu-id="bb0a7-119">名称</span><span class="sxs-lookup"><span data-stu-id="bb0a7-119">Name</span></span>|<span data-ttu-id="bb0a7-120">说明</span><span class="sxs-lookup"><span data-stu-id="bb0a7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bb0a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb0a7-121">Authorization</span></span>|<span data-ttu-id="bb0a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bb0a7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb0a7-124">Content-Type</span></span>|<span data-ttu-id="bb0a7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bb0a7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb0a7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb0a7-127">Request body</span></span>

<span data-ttu-id="bb0a7-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bb0a7-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bb0a7-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="bb0a7-131">属性</span><span class="sxs-lookup"><span data-stu-id="bb0a7-131">Property</span></span>|<span data-ttu-id="bb0a7-132">类型</span><span class="sxs-lookup"><span data-stu-id="bb0a7-132">Type</span></span>|<span data-ttu-id="bb0a7-133">说明</span><span class="sxs-lookup"><span data-stu-id="bb0a7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0a7-134">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="bb0a7-134">applyHoldToSources</span></span>|<span data-ttu-id="bb0a7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb0a7-135">Boolean</span></span>|<span data-ttu-id="bb0a7-136">标识保管人的来源在创建期间是否处于保留状态。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-136">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|

## <a name="response"></a><span data-ttu-id="bb0a7-137">响应</span><span class="sxs-lookup"><span data-stu-id="bb0a7-137">Response</span></span>

<span data-ttu-id="bb0a7-138">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bb0a7-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bb0a7-139">示例</span><span class="sxs-lookup"><span data-stu-id="bb0a7-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb0a7-140">请求</span><span class="sxs-lookup"><span data-stu-id="bb0a7-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bb0a7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb0a7-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_custodian"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
Content-Type: application/json
Content-length: 254

{
  "applyHoldToSources": "false",
}
```
# <a name="c"></a>[<span data-ttu-id="bb0a7-142">C#</span><span class="sxs-lookup"><span data-stu-id="bb0a7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb0a7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb0a7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb0a7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb0a7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb0a7-145">Java</span><span class="sxs-lookup"><span data-stu-id="bb0a7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb0a7-146">响应</span><span class="sxs-lookup"><span data-stu-id="bb0a7-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.custodian"
}
-->

``` http
HTTP/1.1 204 No Content
```
