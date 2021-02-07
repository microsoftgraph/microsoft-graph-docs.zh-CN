---
title: 更新规则
description: 为 messageRule 对象更改可写属性并保存更改。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b7cc38fcc54e73dc177a1a40cc218156f01fbdb8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131584"
---
# <a name="update-rule"></a><span data-ttu-id="bc4e0-103">更新规则</span><span class="sxs-lookup"><span data-stu-id="bc4e0-103">Update rule</span></span>

<span data-ttu-id="bc4e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4e0-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="bc4e0-105">为 [messageRule](../resources/messagerule.md) 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-105">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc4e0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bc4e0-106">Permissions</span></span>
<span data-ttu-id="bc4e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc4e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc4e0-109">Permission type</span></span>      | <span data-ttu-id="bc4e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc4e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc4e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc4e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc4e0-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc4e0-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bc4e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc4e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc4e0-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc4e0-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bc4e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc4e0-115">Application</span></span> | <span data-ttu-id="bc4e0-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc4e0-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc4e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc4e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="bc4e0-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="bc4e0-118">Optional request headers</span></span>
| <span data-ttu-id="bc4e0-119">名称</span><span class="sxs-lookup"><span data-stu-id="bc4e0-119">Name</span></span>       | <span data-ttu-id="bc4e0-120">说明</span><span class="sxs-lookup"><span data-stu-id="bc4e0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bc4e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc4e0-121">Authorization</span></span>  | <span data-ttu-id="bc4e0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bc4e0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc4e0-124">Request body</span></span>
<span data-ttu-id="bc4e0-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc4e0-128">属性</span><span class="sxs-lookup"><span data-stu-id="bc4e0-128">Property</span></span>     | <span data-ttu-id="bc4e0-129">类型</span><span class="sxs-lookup"><span data-stu-id="bc4e0-129">Type</span></span>   |<span data-ttu-id="bc4e0-130">说明</span><span class="sxs-lookup"><span data-stu-id="bc4e0-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc4e0-131">actions</span><span class="sxs-lookup"><span data-stu-id="bc4e0-131">actions</span></span> | [<span data-ttu-id="bc4e0-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="bc4e0-132">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="bc4e0-133">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-133">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="bc4e0-134">conditions</span><span class="sxs-lookup"><span data-stu-id="bc4e0-134">conditions</span></span> | [<span data-ttu-id="bc4e0-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="bc4e0-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="bc4e0-136">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="bc4e0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bc4e0-137">displayName</span></span> | <span data-ttu-id="bc4e0-138">String</span><span class="sxs-lookup"><span data-stu-id="bc4e0-138">String</span></span> | <span data-ttu-id="bc4e0-139">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-139">The display name of the rule.</span></span> |
| <span data-ttu-id="bc4e0-140">exceptions</span><span class="sxs-lookup"><span data-stu-id="bc4e0-140">exceptions</span></span> | [<span data-ttu-id="bc4e0-141">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="bc4e0-141">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="bc4e0-142">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-142">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="bc4e0-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bc4e0-143">isEnabled</span></span> | <span data-ttu-id="bc4e0-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc4e0-144">Boolean</span></span> | <span data-ttu-id="bc4e0-145">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-145">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="bc4e0-146">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="bc4e0-146">isReadOnly</span></span> | <span data-ttu-id="bc4e0-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc4e0-147">Boolean</span></span> | <span data-ttu-id="bc4e0-148">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-148">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="bc4e0-149">Sequence</span><span class="sxs-lookup"><span data-stu-id="bc4e0-149">sequence</span></span> | <span data-ttu-id="bc4e0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bc4e0-150">Int32</span></span> | <span data-ttu-id="bc4e0-151">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-151">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="bc4e0-152">响应</span><span class="sxs-lookup"><span data-stu-id="bc4e0-152">Response</span></span>
<span data-ttu-id="bc4e0-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-153">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc4e0-154">示例</span><span class="sxs-lookup"><span data-stu-id="bc4e0-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc4e0-155">请求</span><span class="sxs-lookup"><span data-stu-id="bc4e0-155">Request</span></span>
<span data-ttu-id="bc4e0-156">下面的示例更改规则名称，并更改针对[获取规则](messagerule-get.md)[示例](messagerule-get.md#example)中的规则所采取的操作，从转发到一个地址到将其重要性标记为“高”。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-156">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="http"></a>[<span data-ttu-id="bc4e0-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc4e0-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bc4e0-158">C#</span><span class="sxs-lookup"><span data-stu-id="bc4e0-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc4e0-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc4e0-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc4e0-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc4e0-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc4e0-161">Java</span><span class="sxs-lookup"><span data-stu-id="bc4e0-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc4e0-162">响应</span><span class="sxs-lookup"><span data-stu-id="bc4e0-162">Response</span></span>
<span data-ttu-id="bc4e0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc4e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

