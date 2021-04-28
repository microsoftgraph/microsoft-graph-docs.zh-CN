---
title: 创建规则
description: '通过指定一组条件和操作来创建 messageRule 对象。 '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fc840b12296b7a308fde8e5af4e39e025fd53a80
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055923"
---
# <a name="create-rule"></a><span data-ttu-id="0239f-103">创建规则</span><span class="sxs-lookup"><span data-stu-id="0239f-103">Create rule</span></span>

<span data-ttu-id="0239f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0239f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="0239f-105">通过指定一组条件和操作来创建 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0239f-105">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="0239f-106">如果用户收件箱中的传入邮件符合指定条件，Outlook 就会执行这些操作。</span><span class="sxs-lookup"><span data-stu-id="0239f-106">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="0239f-107">权限</span><span class="sxs-lookup"><span data-stu-id="0239f-107">Permissions</span></span>
<span data-ttu-id="0239f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0239f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0239f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0239f-110">Permission type</span></span>      | <span data-ttu-id="0239f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0239f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0239f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0239f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0239f-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0239f-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0239f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0239f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0239f-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0239f-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0239f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0239f-116">Application</span></span> | <span data-ttu-id="0239f-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0239f-117">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="0239f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0239f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="0239f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0239f-119">Request headers</span></span>
| <span data-ttu-id="0239f-120">名称</span><span class="sxs-lookup"><span data-stu-id="0239f-120">Name</span></span>       | <span data-ttu-id="0239f-121">说明</span><span class="sxs-lookup"><span data-stu-id="0239f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0239f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0239f-122">Authorization</span></span>  | <span data-ttu-id="0239f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0239f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0239f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0239f-125">Request body</span></span>
<span data-ttu-id="0239f-126">在请求正文中，提供适用于规则的参数。</span><span class="sxs-lookup"><span data-stu-id="0239f-126">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="0239f-127">以下是在创建规则时通常使用的正文参数。</span><span class="sxs-lookup"><span data-stu-id="0239f-127">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="0239f-128">可以根据情况在请求正文中指定任何其他可写的 **messageRule** 属性。</span><span class="sxs-lookup"><span data-stu-id="0239f-128">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="0239f-129">名称</span><span class="sxs-lookup"><span data-stu-id="0239f-129">Name</span></span>       | <span data-ttu-id="0239f-130">类型</span><span class="sxs-lookup"><span data-stu-id="0239f-130">Type</span></span>|<span data-ttu-id="0239f-131">说明</span><span class="sxs-lookup"><span data-stu-id="0239f-131">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="0239f-132">actions</span><span class="sxs-lookup"><span data-stu-id="0239f-132">actions</span></span>|[<span data-ttu-id="0239f-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="0239f-133">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="0239f-134">满足相应条件（如果有的话）时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="0239f-134">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="0239f-135">必需。</span><span class="sxs-lookup"><span data-stu-id="0239f-135">Required.</span></span>|
|<span data-ttu-id="0239f-136">conditions</span><span class="sxs-lookup"><span data-stu-id="0239f-136">conditions</span></span>|[<span data-ttu-id="0239f-137">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0239f-137">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="0239f-138">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="0239f-138">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="0239f-139">可选。</span><span class="sxs-lookup"><span data-stu-id="0239f-139">Optional.</span></span>|
|<span data-ttu-id="0239f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0239f-140">displayName</span></span>| <span data-ttu-id="0239f-141">String</span><span class="sxs-lookup"><span data-stu-id="0239f-141">String</span></span>  | <span data-ttu-id="0239f-142">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0239f-142">The display name of the rule.</span></span> <span data-ttu-id="0239f-143">必需。</span><span class="sxs-lookup"><span data-stu-id="0239f-143">Required.</span></span>|
|<span data-ttu-id="0239f-144">exceptions</span><span class="sxs-lookup"><span data-stu-id="0239f-144">exceptions</span></span>| [<span data-ttu-id="0239f-145">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0239f-145">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="0239f-146">表示规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="0239f-146">Represents exception conditions for the rule.</span></span> <span data-ttu-id="0239f-147">可选。</span><span class="sxs-lookup"><span data-stu-id="0239f-147">Optional.</span></span> |
|<span data-ttu-id="0239f-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0239f-148">isEnabled</span></span> | <span data-ttu-id="0239f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="0239f-149">Boolean</span></span> | <span data-ttu-id="0239f-150">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="0239f-150">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="0239f-151">可选。</span><span class="sxs-lookup"><span data-stu-id="0239f-151">Optional.</span></span> |
|<span data-ttu-id="0239f-152">Sequence</span><span class="sxs-lookup"><span data-stu-id="0239f-152">sequence</span></span>| <span data-ttu-id="0239f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0239f-153">Int32</span></span> | <span data-ttu-id="0239f-154">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="0239f-154">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="0239f-155">必需。</span><span class="sxs-lookup"><span data-stu-id="0239f-155">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="0239f-156">响应</span><span class="sxs-lookup"><span data-stu-id="0239f-156">Response</span></span>
<span data-ttu-id="0239f-157">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="0239f-157">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0239f-158">示例</span><span class="sxs-lookup"><span data-stu-id="0239f-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0239f-159">请求</span><span class="sxs-lookup"><span data-stu-id="0239f-159">Request</span></span>
<span data-ttu-id="0239f-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0239f-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0239f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="0239f-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
# <a name="c"></a>[<span data-ttu-id="0239f-162">C#</span><span class="sxs-lookup"><span data-stu-id="0239f-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0239f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0239f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0239f-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0239f-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0239f-165">Java</span><span class="sxs-lookup"><span data-stu-id="0239f-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-messagerule-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0239f-166">响应</span><span class="sxs-lookup"><span data-stu-id="0239f-166">Response</span></span>
<span data-ttu-id="0239f-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0239f-167">Here is an example of the response.</span></span> <span data-ttu-id="0239f-168">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0239f-168">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
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
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

