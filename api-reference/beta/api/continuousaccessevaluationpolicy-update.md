---
title: 更新 continuousAccessEvaluationPolicy
description: 更新 continuousAccessEvaluationPolicy 对象的属性。
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 80c08c4b711daa2e79600c20ce11f30cd7879af4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437280"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="c2524-103">更新 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="c2524-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="c2524-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2524-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2524-105">更新 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c2524-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2524-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c2524-106">Permissions</span></span>
<span data-ttu-id="c2524-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2524-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2524-109">Permission type</span></span>                        | <span data-ttu-id="c2524-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2524-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="c2524-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2524-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2524-112">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2524-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="c2524-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2524-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2524-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2524-114">Not supported.</span></span> |
|<span data-ttu-id="c2524-115">Application</span><span class="sxs-lookup"><span data-stu-id="c2524-115">Application</span></span>                            | <span data-ttu-id="c2524-116">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2524-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="c2524-117">此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。</span><span class="sxs-lookup"><span data-stu-id="c2524-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2524-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2524-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="c2524-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2524-119">Request headers</span></span>
|<span data-ttu-id="c2524-120">名称</span><span class="sxs-lookup"><span data-stu-id="c2524-120">Name</span></span>|<span data-ttu-id="c2524-121">说明</span><span class="sxs-lookup"><span data-stu-id="c2524-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c2524-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2524-122">Authorization</span></span>|<span data-ttu-id="c2524-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2524-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c2524-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2524-125">Content-Type</span></span>|<span data-ttu-id="c2524-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c2524-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2524-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2524-128">Request body</span></span>
<span data-ttu-id="c2524-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c2524-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c2524-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c2524-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c2524-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c2524-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="c2524-132">属性</span><span class="sxs-lookup"><span data-stu-id="c2524-132">Property</span></span>|<span data-ttu-id="c2524-133">类型</span><span class="sxs-lookup"><span data-stu-id="c2524-133">Type</span></span>|<span data-ttu-id="c2524-134">说明</span><span class="sxs-lookup"><span data-stu-id="c2524-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2524-135">groups</span><span class="sxs-lookup"><span data-stu-id="c2524-135">groups</span></span>|<span data-ttu-id="c2524-136">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c2524-136">String collection</span></span>|<span data-ttu-id="c2524-137">评估范围内组标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="c2524-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="c2524-138">当集合为空时，所有组都位于范围内。</span><span class="sxs-lookup"><span data-stu-id="c2524-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="c2524-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c2524-139">isEnabled</span></span>|<span data-ttu-id="c2524-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2524-140">Boolean</span></span>| <span data-ttu-id="c2524-141">`true` 指示是否应该执行连续访问评估;否则 `false` 。</span><span class="sxs-lookup"><span data-stu-id="c2524-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="c2524-142">users</span><span class="sxs-lookup"><span data-stu-id="c2524-142">users</span></span>|<span data-ttu-id="c2524-143">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c2524-143">String collection</span></span>|<span data-ttu-id="c2524-144">评估范围内用户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="c2524-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="c2524-145">当集合为空时，所有用户都位于范围内。</span><span class="sxs-lookup"><span data-stu-id="c2524-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="c2524-146">响应</span><span class="sxs-lookup"><span data-stu-id="c2524-146">Response</span></span>

<span data-ttu-id="c2524-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c2524-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2524-149">示例</span><span class="sxs-lookup"><span data-stu-id="c2524-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2524-150">请求</span><span class="sxs-lookup"><span data-stu-id="c2524-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c2524-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2524-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "users": [ "88139f01-1f8d-4c06-ad74-a2544cee9aee" ],
  "groups": [ "9972fb3f-7a40-49f5-85f6-129d9dfbd47a", "ea178055-4713-4d9a-a06c-ff17466b7e77"]
}
```
# <a name="c"></a>[<span data-ttu-id="c2524-152">C#</span><span class="sxs-lookup"><span data-stu-id="c2524-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2524-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2524-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2524-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2524-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2524-155">Java</span><span class="sxs-lookup"><span data-stu-id="c2524-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c2524-156">响应</span><span class="sxs-lookup"><span data-stu-id="c2524-156">Response</span></span>

<span data-ttu-id="c2524-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c2524-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
