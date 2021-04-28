---
title: 更新 groupLifecyclePolicy
description: 更新 groupLifecyclePolicy 资源类型对象的属性。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e5c422287c241f2ce9d9d1507114e8795df0dd5e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053060"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="f991f-103">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f991f-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="f991f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f991f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f991f-105">更新 [groupLifecyclePolicy 资源类型](../resources/grouplifecyclepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f991f-105">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f991f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f991f-106">Permissions</span></span>

<span data-ttu-id="f991f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f991f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="f991f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f991f-109">Permission type</span></span>      | <span data-ttu-id="f991f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f991f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f991f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f991f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f991f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f991f-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f991f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f991f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f991f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f991f-114">Not supported.</span></span>    |
|<span data-ttu-id="f991f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f991f-115">Application</span></span> | <span data-ttu-id="f991f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f991f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f991f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f991f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f991f-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f991f-118">Optional request headers</span></span>
| <span data-ttu-id="f991f-119">名称</span><span class="sxs-lookup"><span data-stu-id="f991f-119">Name</span></span> | <span data-ttu-id="f991f-120">说明</span><span class="sxs-lookup"><span data-stu-id="f991f-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="f991f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f991f-121">Authorization</span></span> | <span data-ttu-id="f991f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f991f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f991f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f991f-124">Content-Type</span></span>  | <span data-ttu-id="f991f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f991f-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f991f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f991f-126">Request body</span></span>

<span data-ttu-id="f991f-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f991f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f991f-128">未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f991f-128">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="f991f-129">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="f991f-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f991f-130">属性</span><span class="sxs-lookup"><span data-stu-id="f991f-130">Property</span></span> | <span data-ttu-id="f991f-131">类型</span><span class="sxs-lookup"><span data-stu-id="f991f-131">Type</span></span> | <span data-ttu-id="f991f-132">说明</span><span class="sxs-lookup"><span data-stu-id="f991f-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f991f-133">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f991f-133">alternateNotificationEmails</span></span>|<span data-ttu-id="f991f-134">String</span><span class="sxs-lookup"><span data-stu-id="f991f-134">String</span></span>| <span data-ttu-id="f991f-135">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="f991f-135">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="f991f-136">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f991f-136">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="f991f-137">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="f991f-137">groupLifetimeInDays</span></span>|<span data-ttu-id="f991f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f991f-138">Int32</span></span>| <span data-ttu-id="f991f-139">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="f991f-139">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="f991f-140">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="f991f-140">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="f991f-141">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="f991f-141">managedGroupTypes</span></span>|<span data-ttu-id="f991f-142">String</span><span class="sxs-lookup"><span data-stu-id="f991f-142">String</span></span>| <span data-ttu-id="f991f-143">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="f991f-143">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="f991f-144">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="f991f-144">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="f991f-145">响应</span><span class="sxs-lookup"><span data-stu-id="f991f-145">Response</span></span>

<span data-ttu-id="f991f-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f991f-146">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f991f-147">示例</span><span class="sxs-lookup"><span data-stu-id="f991f-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f991f-148">请求</span><span class="sxs-lookup"><span data-stu-id="f991f-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f991f-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f991f-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="f991f-150">C#</span><span class="sxs-lookup"><span data-stu-id="f991f-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f991f-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f991f-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f991f-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f991f-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f991f-153">Java</span><span class="sxs-lookup"><span data-stu-id="f991f-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f991f-154">响应</span><span class="sxs-lookup"><span data-stu-id="f991f-154">Response</span></span>
<span data-ttu-id="f991f-155">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f991f-155">Note: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

