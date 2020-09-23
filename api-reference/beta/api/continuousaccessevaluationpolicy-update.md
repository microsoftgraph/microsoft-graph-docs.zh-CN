---
title: 更新 continuousAccessEvaluationPolicy
description: 更新 continuousAccessEvaluationPolicy 对象的属性。
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2838a02481690db3d81fd544e88fce65b2053495
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223135"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="8bb86-103">更新 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="8bb86-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="8bb86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bb86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb86-105">更新 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8bb86-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb86-106">权限</span><span class="sxs-lookup"><span data-stu-id="8bb86-106">Permissions</span></span>
<span data-ttu-id="8bb86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bb86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb86-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bb86-109">Permission type</span></span>                        | <span data-ttu-id="8bb86-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bb86-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="8bb86-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bb86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bb86-112">Policy. All、ConditionalAccess 和 Application。 Read. All</span><span class="sxs-lookup"><span data-stu-id="8bb86-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="8bb86-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bb86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb86-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bb86-114">Not supported.</span></span> |
|<span data-ttu-id="8bb86-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bb86-115">Application</span></span>                            | <span data-ttu-id="8bb86-116">Policy. All、ConditionalAccess 和 Application。 Read. All</span><span class="sxs-lookup"><span data-stu-id="8bb86-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="8bb86-117">此 API 存在与权限相关的 [已知问题](/graph/known-issues#permissions) 。</span><span class="sxs-lookup"><span data-stu-id="8bb86-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8bb86-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bb86-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="8bb86-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bb86-119">Request headers</span></span>
|<span data-ttu-id="8bb86-120">名称</span><span class="sxs-lookup"><span data-stu-id="8bb86-120">Name</span></span>|<span data-ttu-id="8bb86-121">说明</span><span class="sxs-lookup"><span data-stu-id="8bb86-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8bb86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bb86-122">Authorization</span></span>|<span data-ttu-id="8bb86-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bb86-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8bb86-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bb86-125">Content-Type</span></span>|<span data-ttu-id="8bb86-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8bb86-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb86-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bb86-128">Request body</span></span>
<span data-ttu-id="8bb86-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8bb86-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8bb86-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8bb86-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8bb86-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8bb86-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="8bb86-132">属性</span><span class="sxs-lookup"><span data-stu-id="8bb86-132">Property</span></span>|<span data-ttu-id="8bb86-133">类型</span><span class="sxs-lookup"><span data-stu-id="8bb86-133">Type</span></span>|<span data-ttu-id="8bb86-134">说明</span><span class="sxs-lookup"><span data-stu-id="8bb86-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb86-135">groups</span><span class="sxs-lookup"><span data-stu-id="8bb86-135">groups</span></span>|<span data-ttu-id="8bb86-136">String collection</span><span class="sxs-lookup"><span data-stu-id="8bb86-136">String collection</span></span>|<span data-ttu-id="8bb86-137">用于评估的范围内的组标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="8bb86-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="8bb86-138">当集合为空时，所有组都在范围内。</span><span class="sxs-lookup"><span data-stu-id="8bb86-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="8bb86-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8bb86-139">isEnabled</span></span>|<span data-ttu-id="8bb86-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb86-140">Boolean</span></span>| <span data-ttu-id="8bb86-141">`true` 以指示是否应执行连续访问评估;否则为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="8bb86-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="8bb86-142">users</span><span class="sxs-lookup"><span data-stu-id="8bb86-142">users</span></span>|<span data-ttu-id="8bb86-143">String collection</span><span class="sxs-lookup"><span data-stu-id="8bb86-143">String collection</span></span>|<span data-ttu-id="8bb86-144">评估范围内的用户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="8bb86-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="8bb86-145">当集合为空时，所有用户都在范围内。</span><span class="sxs-lookup"><span data-stu-id="8bb86-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="8bb86-146">响应</span><span class="sxs-lookup"><span data-stu-id="8bb86-146">Response</span></span>

<span data-ttu-id="8bb86-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8bb86-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bb86-149">示例</span><span class="sxs-lookup"><span data-stu-id="8bb86-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bb86-150">请求</span><span class="sxs-lookup"><span data-stu-id="8bb86-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb86-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb86-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8bb86-152">C#</span><span class="sxs-lookup"><span data-stu-id="8bb86-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb86-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb86-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb86-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb86-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8bb86-155">响应</span><span class="sxs-lookup"><span data-stu-id="8bb86-155">Response</span></span>

<span data-ttu-id="8bb86-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8bb86-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
