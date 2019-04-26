---
title: 创建规则
description: '通过指定一组条件和操作来创建 messageRule 对象。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d48939abdeb124543a6e0db1408afe550f9140d6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338601"
---
# <a name="create-rule"></a><span data-ttu-id="697af-103">创建规则</span><span class="sxs-lookup"><span data-stu-id="697af-103">Create rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="697af-104">通过指定一组条件和操作来创建 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="697af-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="697af-105">如果用户收件箱中的传入邮件符合指定条件，Outlook 就会执行这些操作。</span><span class="sxs-lookup"><span data-stu-id="697af-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="697af-106">权限</span><span class="sxs-lookup"><span data-stu-id="697af-106">Permissions</span></span>
<span data-ttu-id="697af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="697af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="697af-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="697af-109">Permission type</span></span>      | <span data-ttu-id="697af-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="697af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="697af-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="697af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="697af-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="697af-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="697af-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="697af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="697af-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="697af-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="697af-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="697af-115">Application</span></span> | <span data-ttu-id="697af-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="697af-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="697af-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="697af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="697af-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="697af-118">Request headers</span></span>
| <span data-ttu-id="697af-119">名称</span><span class="sxs-lookup"><span data-stu-id="697af-119">Name</span></span>       | <span data-ttu-id="697af-120">说明</span><span class="sxs-lookup"><span data-stu-id="697af-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="697af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="697af-121">Authorization</span></span>  | <span data-ttu-id="697af-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="697af-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="697af-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="697af-124">Request body</span></span>
<span data-ttu-id="697af-125">在请求正文中，提供适用于规则的参数。</span><span class="sxs-lookup"><span data-stu-id="697af-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="697af-126">以下是在创建规则时通常使用的正文参数。</span><span class="sxs-lookup"><span data-stu-id="697af-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="697af-127">可以根据情况在请求正文中指定任何其他可写的 **messageRule** 属性。</span><span class="sxs-lookup"><span data-stu-id="697af-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="697af-128">参数</span><span class="sxs-lookup"><span data-stu-id="697af-128">Parameter</span></span>       | <span data-ttu-id="697af-129">类型</span><span class="sxs-lookup"><span data-stu-id="697af-129">Type</span></span>|<span data-ttu-id="697af-130">说明</span><span class="sxs-lookup"><span data-stu-id="697af-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="697af-131">actions</span><span class="sxs-lookup"><span data-stu-id="697af-131">actions</span></span>|[<span data-ttu-id="697af-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="697af-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="697af-133">满足相应条件（如果有的话）时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="697af-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="697af-134">必需。</span><span class="sxs-lookup"><span data-stu-id="697af-134">Required.</span></span>|
|<span data-ttu-id="697af-135">conditions</span><span class="sxs-lookup"><span data-stu-id="697af-135">conditions</span></span>|[<span data-ttu-id="697af-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="697af-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="697af-137">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="697af-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="697af-138">可选。</span><span class="sxs-lookup"><span data-stu-id="697af-138">Optional.</span></span>|
|<span data-ttu-id="697af-139">displayName</span><span class="sxs-lookup"><span data-stu-id="697af-139">displayName</span></span>| <span data-ttu-id="697af-140">String</span><span class="sxs-lookup"><span data-stu-id="697af-140">String</span></span>  | <span data-ttu-id="697af-141">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="697af-141">The display name of the rule.</span></span> <span data-ttu-id="697af-142">必需。</span><span class="sxs-lookup"><span data-stu-id="697af-142">Required.</span></span>|
|<span data-ttu-id="697af-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="697af-143">exceptions</span></span>| [<span data-ttu-id="697af-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="697af-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="697af-145">表示规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="697af-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="697af-146">可选。</span><span class="sxs-lookup"><span data-stu-id="697af-146">Optional.</span></span> |
|<span data-ttu-id="697af-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="697af-147">isEnabled</span></span> | <span data-ttu-id="697af-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="697af-148">Boolean</span></span> | <span data-ttu-id="697af-149">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="697af-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="697af-150">可选。</span><span class="sxs-lookup"><span data-stu-id="697af-150">Optional.</span></span> |
|<span data-ttu-id="697af-151">Sequence</span><span class="sxs-lookup"><span data-stu-id="697af-151">sequence</span></span>| <span data-ttu-id="697af-152">Int32</span><span class="sxs-lookup"><span data-stu-id="697af-152">Int32</span></span> | <span data-ttu-id="697af-153">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="697af-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="697af-154">必需。</span><span class="sxs-lookup"><span data-stu-id="697af-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="697af-155">响应</span><span class="sxs-lookup"><span data-stu-id="697af-155">Response</span></span>
<span data-ttu-id="697af-156">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="697af-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="697af-157">示例</span><span class="sxs-lookup"><span data-stu-id="697af-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="697af-158">请求</span><span class="sxs-lookup"><span data-stu-id="697af-158">Request</span></span>
<span data-ttu-id="697af-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="697af-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
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
##### <a name="response"></a><span data-ttu-id="697af-160">响应</span><span class="sxs-lookup"><span data-stu-id="697af-160">Response</span></span>
<span data-ttu-id="697af-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="697af-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
