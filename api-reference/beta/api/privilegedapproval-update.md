---
title: 更新 privilegedapproval
description: 更新 privilegedapproval 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e2782b4756ece02695049c4327b651a1796c77c7
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787381"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="3f7f5-103">更新 privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="3f7f5-103">Update privilegedapproval</span></span>

<span data-ttu-id="3f7f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f7f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f7f5-105">更新 privilegedapproval 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-105">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f7f5-106">权限</span><span class="sxs-lookup"><span data-stu-id="3f7f5-106">Permissions</span></span>
<span data-ttu-id="3f7f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3f7f5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f7f5-109">Permission type</span></span>      | <span data-ttu-id="3f7f5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f7f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f7f5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f7f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f7f5-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f7f5-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f7f5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f7f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f7f5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-114">Not supported.</span></span>    |
|<span data-ttu-id="3f7f5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f7f5-115">Application</span></span> | <span data-ttu-id="3f7f5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f7f5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f7f5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3f7f5-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="3f7f5-118">Optional request headers</span></span>
| <span data-ttu-id="3f7f5-119">名称</span><span class="sxs-lookup"><span data-stu-id="3f7f5-119">Name</span></span>       | <span data-ttu-id="3f7f5-120">说明</span><span class="sxs-lookup"><span data-stu-id="3f7f5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3f7f5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f7f5-121">Authorization</span></span>  | <span data-ttu-id="3f7f5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f7f5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f7f5-124">Request body</span></span>
<span data-ttu-id="3f7f5-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3f7f5-128">属性</span><span class="sxs-lookup"><span data-stu-id="3f7f5-128">Property</span></span>     | <span data-ttu-id="3f7f5-129">类型</span><span class="sxs-lookup"><span data-stu-id="3f7f5-129">Type</span></span>   |<span data-ttu-id="3f7f5-130">说明</span><span class="sxs-lookup"><span data-stu-id="3f7f5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f7f5-131">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="3f7f5-131">approvalDuration</span></span>|<span data-ttu-id="3f7f5-132">期限</span><span class="sxs-lookup"><span data-stu-id="3f7f5-132">Duration</span></span>||
|<span data-ttu-id="3f7f5-133">approvalState</span><span class="sxs-lookup"><span data-stu-id="3f7f5-133">approvalState</span></span>|<span data-ttu-id="3f7f5-134">string</span><span class="sxs-lookup"><span data-stu-id="3f7f5-134">string</span></span>| <span data-ttu-id="3f7f5-135">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-135">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="3f7f5-136">approvalType</span><span class="sxs-lookup"><span data-stu-id="3f7f5-136">approvalType</span></span>|<span data-ttu-id="3f7f5-137">String</span><span class="sxs-lookup"><span data-stu-id="3f7f5-137">String</span></span>||
|<span data-ttu-id="3f7f5-138">approverReason</span><span class="sxs-lookup"><span data-stu-id="3f7f5-138">approverReason</span></span>|<span data-ttu-id="3f7f5-139">String</span><span class="sxs-lookup"><span data-stu-id="3f7f5-139">String</span></span>||
|<span data-ttu-id="3f7f5-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3f7f5-140">endDateTime</span></span>|<span data-ttu-id="3f7f5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f7f5-141">DateTimeOffset</span></span>||
|<span data-ttu-id="3f7f5-142">requestorReason</span><span class="sxs-lookup"><span data-stu-id="3f7f5-142">requestorReason</span></span>|<span data-ttu-id="3f7f5-143">String</span><span class="sxs-lookup"><span data-stu-id="3f7f5-143">String</span></span>||
|<span data-ttu-id="3f7f5-144">roleId</span><span class="sxs-lookup"><span data-stu-id="3f7f5-144">roleId</span></span>|<span data-ttu-id="3f7f5-145">String</span><span class="sxs-lookup"><span data-stu-id="3f7f5-145">String</span></span>||
|<span data-ttu-id="3f7f5-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3f7f5-146">startDateTime</span></span>|<span data-ttu-id="3f7f5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f7f5-147">DateTimeOffset</span></span>||
|<span data-ttu-id="3f7f5-148">userId</span><span class="sxs-lookup"><span data-stu-id="3f7f5-148">userId</span></span>|<span data-ttu-id="3f7f5-149">String</span><span class="sxs-lookup"><span data-stu-id="3f7f5-149">String</span></span>||

## <a name="response"></a><span data-ttu-id="3f7f5-150">响应</span><span class="sxs-lookup"><span data-stu-id="3f7f5-150">Response</span></span>

<span data-ttu-id="3f7f5-151">如果成功，此方法返回 `204 No Content` 响应代码</span><span class="sxs-lookup"><span data-stu-id="3f7f5-151">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="3f7f5-152">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3f7f5-153">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="3f7f5-154">示例</span><span class="sxs-lookup"><span data-stu-id="3f7f5-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f7f5-155">请求</span><span class="sxs-lookup"><span data-stu-id="3f7f5-155">Request</span></span>
<span data-ttu-id="3f7f5-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f7f5-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f7f5-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3f7f5-158">C#</span><span class="sxs-lookup"><span data-stu-id="3f7f5-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f7f5-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f7f5-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f7f5-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f7f5-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f7f5-161">Java</span><span class="sxs-lookup"><span data-stu-id="3f7f5-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3f7f5-162">响应</span><span class="sxs-lookup"><span data-stu-id="3f7f5-162">Response</span></span>
<span data-ttu-id="3f7f5-p105">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3f7f5-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


