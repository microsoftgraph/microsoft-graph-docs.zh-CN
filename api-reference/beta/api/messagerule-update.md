---
title: 更新规则
description: 为 messageRule 对象更改可写属性并保存更改。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fbe28b13276c4e5b1debae51a95d9a1655eff93f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050120"
---
# <a name="update-rule"></a><span data-ttu-id="0f3c1-103">更新规则</span><span class="sxs-lookup"><span data-stu-id="0f3c1-103">Update rule</span></span>

<span data-ttu-id="0f3c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f3c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f3c1-105">为 [messageRule](../resources/messagerule.md) 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-105">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f3c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="0f3c1-106">Permissions</span></span>
<span data-ttu-id="0f3c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f3c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f3c1-109">Permission type</span></span>      | <span data-ttu-id="0f3c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f3c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f3c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f3c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f3c1-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f3c1-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0f3c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f3c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f3c1-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f3c1-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0f3c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f3c1-115">Application</span></span> | <span data-ttu-id="0f3c1-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f3c1-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f3c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f3c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0f3c1-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0f3c1-118">Optional request headers</span></span>
| <span data-ttu-id="0f3c1-119">名称</span><span class="sxs-lookup"><span data-stu-id="0f3c1-119">Name</span></span>       | <span data-ttu-id="0f3c1-120">说明</span><span class="sxs-lookup"><span data-stu-id="0f3c1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0f3c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f3c1-121">Authorization</span></span>  | <span data-ttu-id="0f3c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0f3c1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f3c1-124">Request body</span></span>
<span data-ttu-id="0f3c1-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0f3c1-128">属性</span><span class="sxs-lookup"><span data-stu-id="0f3c1-128">Property</span></span>     | <span data-ttu-id="0f3c1-129">类型</span><span class="sxs-lookup"><span data-stu-id="0f3c1-129">Type</span></span>   |<span data-ttu-id="0f3c1-130">说明</span><span class="sxs-lookup"><span data-stu-id="0f3c1-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f3c1-131">actions</span><span class="sxs-lookup"><span data-stu-id="0f3c1-131">actions</span></span> | [<span data-ttu-id="0f3c1-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="0f3c1-132">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="0f3c1-133">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-133">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="0f3c1-134">conditions</span><span class="sxs-lookup"><span data-stu-id="0f3c1-134">conditions</span></span> | [<span data-ttu-id="0f3c1-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0f3c1-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="0f3c1-136">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="0f3c1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0f3c1-137">displayName</span></span> | <span data-ttu-id="0f3c1-138">String</span><span class="sxs-lookup"><span data-stu-id="0f3c1-138">String</span></span> | <span data-ttu-id="0f3c1-139">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-139">The display name of the rule.</span></span> |
| <span data-ttu-id="0f3c1-140">exceptions</span><span class="sxs-lookup"><span data-stu-id="0f3c1-140">exceptions</span></span> | [<span data-ttu-id="0f3c1-141">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0f3c1-141">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="0f3c1-142">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-142">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="0f3c1-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0f3c1-143">isEnabled</span></span> | <span data-ttu-id="0f3c1-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3c1-144">Boolean</span></span> | <span data-ttu-id="0f3c1-145">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-145">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="0f3c1-146">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="0f3c1-146">isReadOnly</span></span> | <span data-ttu-id="0f3c1-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3c1-147">Boolean</span></span> | <span data-ttu-id="0f3c1-148">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-148">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="0f3c1-149">Sequence</span><span class="sxs-lookup"><span data-stu-id="0f3c1-149">sequence</span></span> | <span data-ttu-id="0f3c1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0f3c1-150">Int32</span></span> | <span data-ttu-id="0f3c1-151">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-151">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="0f3c1-152">响应</span><span class="sxs-lookup"><span data-stu-id="0f3c1-152">Response</span></span>
<span data-ttu-id="0f3c1-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-153">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f3c1-154">示例</span><span class="sxs-lookup"><span data-stu-id="0f3c1-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f3c1-155">请求</span><span class="sxs-lookup"><span data-stu-id="0f3c1-155">Request</span></span>
<span data-ttu-id="0f3c1-156">下面的示例更改规则名称，并更改针对[获取规则](messagerule-get.md)[示例](messagerule-get.md#example)中的规则所采取的操作，从转发到一个地址到将其重要性标记为“高”。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-156">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="http"></a>[<span data-ttu-id="0f3c1-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f3c1-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
# <a name="c"></a>[<span data-ttu-id="0f3c1-158">C#</span><span class="sxs-lookup"><span data-stu-id="0f3c1-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f3c1-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f3c1-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f3c1-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f3c1-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f3c1-161">Java</span><span class="sxs-lookup"><span data-stu-id="0f3c1-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0f3c1-162">响应</span><span class="sxs-lookup"><span data-stu-id="0f3c1-162">Response</span></span>
<span data-ttu-id="0f3c1-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-163">Here is an example of the response.</span></span> <span data-ttu-id="0f3c1-164">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0f3c1-164">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


