---
title: 更新规则
description: 为 messageRule 对象更改可写属性并保存更改。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dd81b2cc6be26ae730e388d1df6e72fbdbf10f98
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276732"
---
# <a name="update-rule"></a><span data-ttu-id="c8e11-103">更新规则</span><span class="sxs-lookup"><span data-stu-id="c8e11-103">Update rule</span></span>


<span data-ttu-id="c8e11-104">为 [messageRule](../resources/messagerule.md) 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="c8e11-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e11-105">权限</span><span class="sxs-lookup"><span data-stu-id="c8e11-105">Permissions</span></span>
<span data-ttu-id="c8e11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8e11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e11-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8e11-108">Permission type</span></span>      | <span data-ttu-id="c8e11-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8e11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8e11-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8e11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8e11-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8e11-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c8e11-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8e11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e11-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8e11-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c8e11-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8e11-114">Application</span></span> | <span data-ttu-id="c8e11-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8e11-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8e11-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8e11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c8e11-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c8e11-117">Optional request headers</span></span>
| <span data-ttu-id="c8e11-118">名称</span><span class="sxs-lookup"><span data-stu-id="c8e11-118">Name</span></span>       | <span data-ttu-id="c8e11-119">说明</span><span class="sxs-lookup"><span data-stu-id="c8e11-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c8e11-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8e11-120">Authorization</span></span>  | <span data-ttu-id="c8e11-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8e11-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c8e11-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8e11-123">Request body</span></span>
<span data-ttu-id="c8e11-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c8e11-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8e11-127">属性</span><span class="sxs-lookup"><span data-stu-id="c8e11-127">Property</span></span>     | <span data-ttu-id="c8e11-128">类型</span><span class="sxs-lookup"><span data-stu-id="c8e11-128">Type</span></span>   |<span data-ttu-id="c8e11-129">说明</span><span class="sxs-lookup"><span data-stu-id="c8e11-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c8e11-130">actions</span><span class="sxs-lookup"><span data-stu-id="c8e11-130">actions</span></span> | [<span data-ttu-id="c8e11-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="c8e11-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="c8e11-132">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="c8e11-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="c8e11-133">conditions</span><span class="sxs-lookup"><span data-stu-id="c8e11-133">conditions</span></span> | [<span data-ttu-id="c8e11-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="c8e11-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="c8e11-135">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="c8e11-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="c8e11-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c8e11-136">displayName</span></span> | <span data-ttu-id="c8e11-137">String</span><span class="sxs-lookup"><span data-stu-id="c8e11-137">String</span></span> | <span data-ttu-id="c8e11-138">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c8e11-138">The display name of the rule.</span></span> |
| <span data-ttu-id="c8e11-139">exceptions</span><span class="sxs-lookup"><span data-stu-id="c8e11-139">exceptions</span></span> | [<span data-ttu-id="c8e11-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="c8e11-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="c8e11-141">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="c8e11-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="c8e11-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c8e11-142">isEnabled</span></span> | <span data-ttu-id="c8e11-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8e11-143">Boolean</span></span> | <span data-ttu-id="c8e11-144">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="c8e11-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="c8e11-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="c8e11-145">isReadOnly</span></span> | <span data-ttu-id="c8e11-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8e11-146">Boolean</span></span> | <span data-ttu-id="c8e11-147">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="c8e11-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="c8e11-148">Sequence</span><span class="sxs-lookup"><span data-stu-id="c8e11-148">sequence</span></span> | <span data-ttu-id="c8e11-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c8e11-149">Int32</span></span> | <span data-ttu-id="c8e11-150">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="c8e11-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="c8e11-151">响应</span><span class="sxs-lookup"><span data-stu-id="c8e11-151">Response</span></span>
<span data-ttu-id="c8e11-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8e11-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8e11-153">示例</span><span class="sxs-lookup"><span data-stu-id="c8e11-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8e11-154">请求</span><span class="sxs-lookup"><span data-stu-id="c8e11-154">Request</span></span>
<span data-ttu-id="c8e11-155">下面的示例更改规则名称，并更改针对[获取规则](messagerule-get.md)[示例](messagerule-get.md#example)中的规则所采取的操作，从转发到一个地址到将其重要性标记为“高”。</span><span class="sxs-lookup"><span data-stu-id="c8e11-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
##### <a name="response"></a><span data-ttu-id="c8e11-156">响应</span><span class="sxs-lookup"><span data-stu-id="c8e11-156">Response</span></span>
<span data-ttu-id="c8e11-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8e11-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c8e11-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c8e11-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c8e11-161">C#</span><span class="sxs-lookup"><span data-stu-id="c8e11-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_messagerule-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8e11-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8e11-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_messagerule-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c8e11-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="c8e11-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_messagerule-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/messagerule-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/messagerule-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/messagerule-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
