---
title: 更新 continuousAccessEvaluationPolicy
description: 更新 continuousAccessEvaluationPolicy 对象的属性。
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 990428fc0022bca7d27f6eaac7978071f49381cb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956935"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="5cb3e-103">更新 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="5cb3e-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="5cb3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cb3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cb3e-105">更新 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cb3e-106">权限</span><span class="sxs-lookup"><span data-stu-id="5cb3e-106">Permissions</span></span>
<span data-ttu-id="5cb3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cb3e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cb3e-109">Permission type</span></span>                        | <span data-ttu-id="5cb3e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cb3e-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="5cb3e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cb3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cb3e-112">Policy. All、ConditionalAccess 和 Application。 Read. All</span><span class="sxs-lookup"><span data-stu-id="5cb3e-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="5cb3e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cb3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cb3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-114">Not supported.</span></span> |
|<span data-ttu-id="5cb3e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cb3e-115">Application</span></span>                            | <span data-ttu-id="5cb3e-116">Policy. All、ConditionalAccess 和 Application。 Read. All</span><span class="sxs-lookup"><span data-stu-id="5cb3e-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="5cb3e-117">此 API 存在与权限相关的 [已知问题](/graph/known-issues#permissions) 。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="5cb3e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cb3e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="5cb3e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cb3e-119">Request headers</span></span>
|<span data-ttu-id="5cb3e-120">名称</span><span class="sxs-lookup"><span data-stu-id="5cb3e-120">Name</span></span>|<span data-ttu-id="5cb3e-121">说明</span><span class="sxs-lookup"><span data-stu-id="5cb3e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5cb3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cb3e-122">Authorization</span></span>|<span data-ttu-id="5cb3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5cb3e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cb3e-125">Content-Type</span></span>|<span data-ttu-id="5cb3e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5cb3e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cb3e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cb3e-128">Request body</span></span>
<span data-ttu-id="5cb3e-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5cb3e-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5cb3e-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="5cb3e-132">属性</span><span class="sxs-lookup"><span data-stu-id="5cb3e-132">Property</span></span>|<span data-ttu-id="5cb3e-133">类型</span><span class="sxs-lookup"><span data-stu-id="5cb3e-133">Type</span></span>|<span data-ttu-id="5cb3e-134">说明</span><span class="sxs-lookup"><span data-stu-id="5cb3e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cb3e-135">groups</span><span class="sxs-lookup"><span data-stu-id="5cb3e-135">groups</span></span>|<span data-ttu-id="5cb3e-136">String collection</span><span class="sxs-lookup"><span data-stu-id="5cb3e-136">String collection</span></span>|<span data-ttu-id="5cb3e-137">用于评估的范围内的组标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="5cb3e-138">当集合为空时，所有组都在范围内。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="5cb3e-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5cb3e-139">isEnabled</span></span>|<span data-ttu-id="5cb3e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cb3e-140">Boolean</span></span>| <span data-ttu-id="5cb3e-141">`true` 以指示是否应执行连续访问评估;否则为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="5cb3e-142">users</span><span class="sxs-lookup"><span data-stu-id="5cb3e-142">users</span></span>|<span data-ttu-id="5cb3e-143">String collection</span><span class="sxs-lookup"><span data-stu-id="5cb3e-143">String collection</span></span>|<span data-ttu-id="5cb3e-144">评估范围内的用户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="5cb3e-145">当集合为空时，所有用户都在范围内。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="5cb3e-146">响应</span><span class="sxs-lookup"><span data-stu-id="5cb3e-146">Response</span></span>

<span data-ttu-id="5cb3e-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5cb3e-149">示例</span><span class="sxs-lookup"><span data-stu-id="5cb3e-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5cb3e-150">请求</span><span class="sxs-lookup"><span data-stu-id="5cb3e-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5cb3e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cb3e-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5cb3e-152">C#</span><span class="sxs-lookup"><span data-stu-id="5cb3e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cb3e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cb3e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cb3e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cb3e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5cb3e-155">Java</span><span class="sxs-lookup"><span data-stu-id="5cb3e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5cb3e-156">响应</span><span class="sxs-lookup"><span data-stu-id="5cb3e-156">Response</span></span>

<span data-ttu-id="5cb3e-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5cb3e-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
