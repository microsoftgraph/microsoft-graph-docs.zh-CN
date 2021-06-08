---
title: 更新 legalHold
description: 更新 legalHold 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3bee140093a74f335d9316d8785189350ae29f19
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786802"
---
# <a name="update-legalhold"></a><span data-ttu-id="f4579-103">更新 legalHold</span><span class="sxs-lookup"><span data-stu-id="f4579-103">Update legalHold</span></span>

<span data-ttu-id="f4579-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f4579-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4579-105">更新 [legalHold 对象](../resources/ediscovery-legalhold.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f4579-105">Update the properties of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4579-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4579-106">Permissions</span></span>

<span data-ttu-id="f4579-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4579-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4579-109">Permission type</span></span>|<span data-ttu-id="f4579-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4579-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4579-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4579-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4579-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4579-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f4579-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4579-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4579-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4579-114">Not supported.</span></span>|
|<span data-ttu-id="f4579-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4579-115">Application</span></span>|<span data-ttu-id="f4579-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4579-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4579-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4579-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="request-headers"></a><span data-ttu-id="f4579-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4579-118">Request headers</span></span>

|<span data-ttu-id="f4579-119">名称</span><span class="sxs-lookup"><span data-stu-id="f4579-119">Name</span></span>|<span data-ttu-id="f4579-120">说明</span><span class="sxs-lookup"><span data-stu-id="f4579-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4579-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4579-121">Authorization</span></span>|<span data-ttu-id="f4579-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4579-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f4579-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4579-124">Content-Type</span></span>|<span data-ttu-id="f4579-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f4579-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4579-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4579-127">Request body</span></span>

<span data-ttu-id="f4579-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f4579-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f4579-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f4579-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f4579-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f4579-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="f4579-131">属性</span><span class="sxs-lookup"><span data-stu-id="f4579-131">Property</span></span>|<span data-ttu-id="f4579-132">类型</span><span class="sxs-lookup"><span data-stu-id="f4579-132">Type</span></span>|<span data-ttu-id="f4579-133">说明</span><span class="sxs-lookup"><span data-stu-id="f4579-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4579-134">contentQuery</span><span class="sxs-lookup"><span data-stu-id="f4579-134">contentQuery</span></span>|<span data-ttu-id="f4579-135">String</span><span class="sxs-lookup"><span data-stu-id="f4579-135">String</span></span>|<span data-ttu-id="f4579-136">指定要位于指定位置的内容的 KQL 查询。</span><span class="sxs-lookup"><span data-stu-id="f4579-136">KQL query that specifies content to be held in the specified locations.</span></span> <span data-ttu-id="f4579-137">有关电子数据展示中的 KQL 详细信息，请参阅内容搜索和电子数据展示的关键字查询 [和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。</span><span class="sxs-lookup"><span data-stu-id="f4579-137">For more information about KQL in eDiscovery, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span> <span data-ttu-id="f4579-138">若要保留指定位置中所有的内容，请保留 **contentQuery** 为空。</span><span class="sxs-lookup"><span data-stu-id="f4579-138">To hold all content in the specified locations, leave **contentQuery** blank.</span></span> |
|<span data-ttu-id="f4579-139">description</span><span class="sxs-lookup"><span data-stu-id="f4579-139">description</span></span>|<span data-ttu-id="f4579-140">String</span><span class="sxs-lookup"><span data-stu-id="f4579-140">String</span></span>| <span data-ttu-id="f4579-141">法定保留说明。</span><span class="sxs-lookup"><span data-stu-id="f4579-141">The legal hold description.</span></span> |
|<span data-ttu-id="f4579-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f4579-142">displayName</span></span>|<span data-ttu-id="f4579-143">String</span><span class="sxs-lookup"><span data-stu-id="f4579-143">String</span></span>| <span data-ttu-id="f4579-144">法定显示名称的保留项。</span><span class="sxs-lookup"><span data-stu-id="f4579-144">The display name of the legal hold.</span></span> |
|<span data-ttu-id="f4579-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f4579-145">isEnabled</span></span>|<span data-ttu-id="f4579-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4579-146">Boolean</span></span>|<span data-ttu-id="f4579-147">指示是否启用保留并主动保留内容。</span><span class="sxs-lookup"><span data-stu-id="f4579-147">Indicates whether the hold is enabled and actively holding content.</span></span> |

## <a name="response"></a><span data-ttu-id="f4579-148">响应</span><span class="sxs-lookup"><span data-stu-id="f4579-148">Response</span></span>

<span data-ttu-id="f4579-149">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f4579-149">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f4579-150">示例</span><span class="sxs-lookup"><span data-stu-id="f4579-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4579-151">请求</span><span class="sxs-lookup"><span data-stu-id="f4579-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f4579-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4579-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_legalhold"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
Content-Type: application/json
Content-length: 295

{
  "description": "This is a description for a legalHold"
}
```
# <a name="c"></a>[<span data-ttu-id="f4579-153">C#</span><span class="sxs-lookup"><span data-stu-id="f4579-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-legalhold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4579-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4579-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-legalhold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4579-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4579-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-legalhold-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4579-156">Java</span><span class="sxs-lookup"><span data-stu-id="f4579-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-legalhold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4579-157">响应</span><span class="sxs-lookup"><span data-stu-id="f4579-157">Response</span></span>

<!-- {
  "blockType": "response"
}
-->

``` http
HTTP/1.1 204 No Content
```
