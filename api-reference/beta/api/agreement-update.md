---
title: 更新协议
description: 更新协议对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 77c3fbf6aa37d283e02408a1000d4a5f521a3fd5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048195"
---
# <a name="update-agreement"></a><span data-ttu-id="9cc13-103">更新协议</span><span class="sxs-lookup"><span data-stu-id="9cc13-103">Update agreement</span></span>

<span data-ttu-id="9cc13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc13-105">更新 [协议对象的属性](../resources/agreement.md) 。</span><span class="sxs-lookup"><span data-stu-id="9cc13-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cc13-106">权限</span><span class="sxs-lookup"><span data-stu-id="9cc13-106">Permissions</span></span>
<span data-ttu-id="9cc13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cc13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc13-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc13-109">Permission type</span></span>                        | <span data-ttu-id="9cc13-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cc13-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc13-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cc13-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc13-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="9cc13-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc13-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc13-114">Not supported.</span></span> |
|<span data-ttu-id="9cc13-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cc13-115">Application</span></span>                            | <span data-ttu-id="9cc13-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc13-116">Not supported.</span></span> |

<span data-ttu-id="9cc13-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="9cc13-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="9cc13-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="9cc13-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="9cc13-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9cc13-119">Global Administrator</span></span>
+ <span data-ttu-id="9cc13-120">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="9cc13-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="9cc13-121">安全管理员</span><span class="sxs-lookup"><span data-stu-id="9cc13-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9cc13-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc13-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9cc13-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cc13-123">Request headers</span></span>
| <span data-ttu-id="9cc13-124">名称</span><span class="sxs-lookup"><span data-stu-id="9cc13-124">Name</span></span>         | <span data-ttu-id="9cc13-125">类型</span><span class="sxs-lookup"><span data-stu-id="9cc13-125">Type</span></span>        | <span data-ttu-id="9cc13-126">说明</span><span class="sxs-lookup"><span data-stu-id="9cc13-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9cc13-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc13-127">Authorization</span></span> | <span data-ttu-id="9cc13-128">string</span><span class="sxs-lookup"><span data-stu-id="9cc13-128">string</span></span> | <span data-ttu-id="9cc13-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cc13-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cc13-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc13-131">Request body</span></span>
<span data-ttu-id="9cc13-132">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9cc13-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9cc13-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9cc13-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9cc13-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9cc13-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9cc13-135">属性</span><span class="sxs-lookup"><span data-stu-id="9cc13-135">Property</span></span>     | <span data-ttu-id="9cc13-136">类型</span><span class="sxs-lookup"><span data-stu-id="9cc13-136">Type</span></span>        | <span data-ttu-id="9cc13-137">说明</span><span class="sxs-lookup"><span data-stu-id="9cc13-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9cc13-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9cc13-138">displayName</span></span>|<span data-ttu-id="9cc13-139">String</span><span class="sxs-lookup"><span data-stu-id="9cc13-139">String</span></span>|<span data-ttu-id="9cc13-140">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9cc13-140">Display name of the agreement.</span></span>|
|<span data-ttu-id="9cc13-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="9cc13-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="9cc13-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="9cc13-142">Boolean</span></span>|<span data-ttu-id="9cc13-143">用户是否必须展开和查看协议才能接受。</span><span class="sxs-lookup"><span data-stu-id="9cc13-143">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="9cc13-144">响应</span><span class="sxs-lookup"><span data-stu-id="9cc13-144">Response</span></span>
<span data-ttu-id="9cc13-145">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码[](../resources/agreement.md)和更新的协议对象。</span><span class="sxs-lookup"><span data-stu-id="9cc13-145">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cc13-146">示例</span><span class="sxs-lookup"><span data-stu-id="9cc13-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cc13-147">请求</span><span class="sxs-lookup"><span data-stu-id="9cc13-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9cc13-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc13-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="9cc13-149">C#</span><span class="sxs-lookup"><span data-stu-id="9cc13-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc13-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc13-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc13-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc13-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cc13-152">Java</span><span class="sxs-lookup"><span data-stu-id="9cc13-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9cc13-153">响应</span><span class="sxs-lookup"><span data-stu-id="9cc13-153">Response</span></span>
><span data-ttu-id="9cc13-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cc13-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


