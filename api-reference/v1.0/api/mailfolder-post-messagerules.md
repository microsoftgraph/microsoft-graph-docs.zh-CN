---
title: 创建规则
description: '通过指定一组条件和操作来创建 messageRule 对象。 '
author: angelgolfer-ms
ms.openlocfilehash: 72c4991e077364514104d5bbc8e24625526bce51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361353"
---
# <a name="create-rule"></a><span data-ttu-id="140ab-103">创建规则</span><span class="sxs-lookup"><span data-stu-id="140ab-103">Create rule</span></span>


<span data-ttu-id="140ab-104">通过指定一组条件和操作来创建 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="140ab-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="140ab-105">如果用户收件箱中的传入邮件符合指定条件，Outlook 就会执行这些操作。</span><span class="sxs-lookup"><span data-stu-id="140ab-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="140ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="140ab-106">Permissions</span></span>
<span data-ttu-id="140ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="140ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="140ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="140ab-109">Permission type</span></span>      | <span data-ttu-id="140ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="140ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="140ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="140ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="140ab-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="140ab-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="140ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="140ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="140ab-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="140ab-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="140ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="140ab-115">Application</span></span> | <span data-ttu-id="140ab-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="140ab-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="140ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="140ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="140ab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="140ab-118">Request headers</span></span>
| <span data-ttu-id="140ab-119">Name</span><span class="sxs-lookup"><span data-stu-id="140ab-119">Name</span></span>       | <span data-ttu-id="140ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="140ab-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="140ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="140ab-121">Authorization</span></span>  | <span data-ttu-id="140ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="140ab-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="140ab-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="140ab-124">Request body</span></span>
<span data-ttu-id="140ab-125">在请求正文中，提供适用于规则的参数。</span><span class="sxs-lookup"><span data-stu-id="140ab-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="140ab-126">以下是在创建规则时通常使用的正文参数。</span><span class="sxs-lookup"><span data-stu-id="140ab-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="140ab-127">可以根据情况在请求正文中指定任何其他可写的 **messageRule** 属性。</span><span class="sxs-lookup"><span data-stu-id="140ab-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="140ab-128">Name</span><span class="sxs-lookup"><span data-stu-id="140ab-128">Name</span></span>       | <span data-ttu-id="140ab-129">类型</span><span class="sxs-lookup"><span data-stu-id="140ab-129">Type</span></span>|<span data-ttu-id="140ab-130">说明</span><span class="sxs-lookup"><span data-stu-id="140ab-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="140ab-131">actions</span><span class="sxs-lookup"><span data-stu-id="140ab-131">actions</span></span>|[<span data-ttu-id="140ab-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="140ab-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="140ab-133">满足相应条件（如果有的话）时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="140ab-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="140ab-134">必需。</span><span class="sxs-lookup"><span data-stu-id="140ab-134">Required.</span></span>|
|<span data-ttu-id="140ab-135">conditions</span><span class="sxs-lookup"><span data-stu-id="140ab-135">conditions</span></span>|[<span data-ttu-id="140ab-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="140ab-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="140ab-137">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="140ab-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="140ab-138">可选。</span><span class="sxs-lookup"><span data-stu-id="140ab-138">Optional.</span></span>|
|<span data-ttu-id="140ab-139">displayName</span><span class="sxs-lookup"><span data-stu-id="140ab-139">displayName</span></span>| <span data-ttu-id="140ab-140">String</span><span class="sxs-lookup"><span data-stu-id="140ab-140">String</span></span>  | <span data-ttu-id="140ab-141">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="140ab-141">The display name of the rule.</span></span> <span data-ttu-id="140ab-142">必需。</span><span class="sxs-lookup"><span data-stu-id="140ab-142">Required.</span></span>|
|<span data-ttu-id="140ab-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="140ab-143">exceptions</span></span>| [<span data-ttu-id="140ab-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="140ab-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="140ab-145">表示规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="140ab-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="140ab-146">可选。</span><span class="sxs-lookup"><span data-stu-id="140ab-146">Optional.</span></span> |
|<span data-ttu-id="140ab-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="140ab-147">isEnabled</span></span> | <span data-ttu-id="140ab-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="140ab-148">Boolean</span></span> | <span data-ttu-id="140ab-149">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="140ab-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="140ab-150">可选。</span><span class="sxs-lookup"><span data-stu-id="140ab-150">Optional.</span></span> |
|<span data-ttu-id="140ab-151">Sequence</span><span class="sxs-lookup"><span data-stu-id="140ab-151">sequence</span></span>| <span data-ttu-id="140ab-152">Int32</span><span class="sxs-lookup"><span data-stu-id="140ab-152">Int32</span></span> | <span data-ttu-id="140ab-153">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="140ab-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="140ab-154">必需。</span><span class="sxs-lookup"><span data-stu-id="140ab-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="140ab-155">响应</span><span class="sxs-lookup"><span data-stu-id="140ab-155">Response</span></span>
<span data-ttu-id="140ab-156">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="140ab-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="140ab-157">示例</span><span class="sxs-lookup"><span data-stu-id="140ab-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="140ab-158">请求</span><span class="sxs-lookup"><span data-stu-id="140ab-158">Request</span></span>
<span data-ttu-id="140ab-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="140ab-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="140ab-160">响应</span><span class="sxs-lookup"><span data-stu-id="140ab-160">Response</span></span>
<span data-ttu-id="140ab-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="140ab-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->