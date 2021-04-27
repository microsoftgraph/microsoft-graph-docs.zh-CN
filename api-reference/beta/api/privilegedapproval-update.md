---
title: 更新 privilegedapproval
description: 更新 privilegedapproval 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 89d65455ecc1eea427c0e2186a97fbad39789884
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053543"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="fa31a-103">更新 privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="fa31a-103">Update privilegedapproval</span></span>

<span data-ttu-id="fa31a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa31a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa31a-105">更新 privilegedapproval 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa31a-105">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa31a-106">权限</span><span class="sxs-lookup"><span data-stu-id="fa31a-106">Permissions</span></span>
<span data-ttu-id="fa31a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa31a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa31a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa31a-109">Permission type</span></span>      | <span data-ttu-id="fa31a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa31a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa31a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa31a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fa31a-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa31a-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa31a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa31a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa31a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa31a-114">Not supported.</span></span>    |
|<span data-ttu-id="fa31a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa31a-115">Application</span></span> | <span data-ttu-id="fa31a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa31a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa31a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa31a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fa31a-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="fa31a-118">Optional request headers</span></span>
| <span data-ttu-id="fa31a-119">名称</span><span class="sxs-lookup"><span data-stu-id="fa31a-119">Name</span></span>       | <span data-ttu-id="fa31a-120">说明</span><span class="sxs-lookup"><span data-stu-id="fa31a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fa31a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa31a-121">Authorization</span></span>  | <span data-ttu-id="fa31a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa31a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa31a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa31a-124">Request body</span></span>
<span data-ttu-id="fa31a-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fa31a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa31a-128">属性</span><span class="sxs-lookup"><span data-stu-id="fa31a-128">Property</span></span>     | <span data-ttu-id="fa31a-129">类型</span><span class="sxs-lookup"><span data-stu-id="fa31a-129">Type</span></span>   |<span data-ttu-id="fa31a-130">说明</span><span class="sxs-lookup"><span data-stu-id="fa31a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa31a-131">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="fa31a-131">approvalDuration</span></span>|<span data-ttu-id="fa31a-132">期限</span><span class="sxs-lookup"><span data-stu-id="fa31a-132">Duration</span></span>||
|<span data-ttu-id="fa31a-133">approvalState</span><span class="sxs-lookup"><span data-stu-id="fa31a-133">approvalState</span></span>|<span data-ttu-id="fa31a-134">string</span><span class="sxs-lookup"><span data-stu-id="fa31a-134">string</span></span>| <span data-ttu-id="fa31a-135">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="fa31a-135">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="fa31a-136">approvalType</span><span class="sxs-lookup"><span data-stu-id="fa31a-136">approvalType</span></span>|<span data-ttu-id="fa31a-137">String</span><span class="sxs-lookup"><span data-stu-id="fa31a-137">String</span></span>||
|<span data-ttu-id="fa31a-138">approverReason</span><span class="sxs-lookup"><span data-stu-id="fa31a-138">approverReason</span></span>|<span data-ttu-id="fa31a-139">String</span><span class="sxs-lookup"><span data-stu-id="fa31a-139">String</span></span>||
|<span data-ttu-id="fa31a-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fa31a-140">endDateTime</span></span>|<span data-ttu-id="fa31a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa31a-141">DateTimeOffset</span></span>||
|<span data-ttu-id="fa31a-142">requestorReason</span><span class="sxs-lookup"><span data-stu-id="fa31a-142">requestorReason</span></span>|<span data-ttu-id="fa31a-143">String</span><span class="sxs-lookup"><span data-stu-id="fa31a-143">String</span></span>||
|<span data-ttu-id="fa31a-144">roleId</span><span class="sxs-lookup"><span data-stu-id="fa31a-144">roleId</span></span>|<span data-ttu-id="fa31a-145">String</span><span class="sxs-lookup"><span data-stu-id="fa31a-145">String</span></span>||
|<span data-ttu-id="fa31a-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fa31a-146">startDateTime</span></span>|<span data-ttu-id="fa31a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa31a-147">DateTimeOffset</span></span>||
|<span data-ttu-id="fa31a-148">userId</span><span class="sxs-lookup"><span data-stu-id="fa31a-148">userId</span></span>|<span data-ttu-id="fa31a-149">String</span><span class="sxs-lookup"><span data-stu-id="fa31a-149">String</span></span>||

## <a name="response"></a><span data-ttu-id="fa31a-150">响应</span><span class="sxs-lookup"><span data-stu-id="fa31a-150">Response</span></span>

<span data-ttu-id="fa31a-151">如果成功，此方法返回 `204 No Content` 响应代码</span><span class="sxs-lookup"><span data-stu-id="fa31a-151">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="fa31a-152">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="fa31a-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="fa31a-153">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="fa31a-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="fa31a-154">示例</span><span class="sxs-lookup"><span data-stu-id="fa31a-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa31a-155">请求</span><span class="sxs-lookup"><span data-stu-id="fa31a-155">Request</span></span>
<span data-ttu-id="fa31a-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa31a-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa31a-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa31a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval/{requestId}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
# <a name="c"></a>[<span data-ttu-id="fa31a-158">C#</span><span class="sxs-lookup"><span data-stu-id="fa31a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa31a-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa31a-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa31a-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa31a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa31a-161">Java</span><span class="sxs-lookup"><span data-stu-id="fa31a-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa31a-162">响应</span><span class="sxs-lookup"><span data-stu-id="fa31a-162">Response</span></span>
<span data-ttu-id="fa31a-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fa31a-163">Here is an example of the response.</span></span> <span data-ttu-id="fa31a-164">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fa31a-164">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


