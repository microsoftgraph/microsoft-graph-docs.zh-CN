---
title: 创建规则
description: '通过指定一组条件和操作来创建 messageRule 对象。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c21ab70c723e9a97711e87559dc06856672fee0f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970421"
---
# <a name="create-rule"></a><span data-ttu-id="404b3-103">创建规则</span><span class="sxs-lookup"><span data-stu-id="404b3-103">Create rule</span></span>

> <span data-ttu-id="404b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="404b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="404b3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="404b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="404b3-106">通过指定一组条件和操作来创建 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="404b3-106">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="404b3-107">如果用户收件箱中的传入邮件符合指定条件，Outlook 就会执行这些操作。</span><span class="sxs-lookup"><span data-stu-id="404b3-107">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="404b3-108">权限</span><span class="sxs-lookup"><span data-stu-id="404b3-108">Permissions</span></span>
<span data-ttu-id="404b3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="404b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="404b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="404b3-111">Permission type</span></span>      | <span data-ttu-id="404b3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="404b3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="404b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="404b3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="404b3-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="404b3-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="404b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="404b3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="404b3-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="404b3-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="404b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="404b3-117">Application</span></span> | <span data-ttu-id="404b3-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="404b3-118">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="404b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="404b3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="404b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="404b3-120">Request headers</span></span>
| <span data-ttu-id="404b3-121">名称</span><span class="sxs-lookup"><span data-stu-id="404b3-121">Name</span></span>       | <span data-ttu-id="404b3-122">说明</span><span class="sxs-lookup"><span data-stu-id="404b3-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="404b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="404b3-123">Authorization</span></span>  | <span data-ttu-id="404b3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="404b3-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="404b3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="404b3-126">Request body</span></span>
<span data-ttu-id="404b3-127">在请求正文中，提供适用于规则的参数。</span><span class="sxs-lookup"><span data-stu-id="404b3-127">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="404b3-128">以下是在创建规则时通常使用的正文参数。</span><span class="sxs-lookup"><span data-stu-id="404b3-128">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="404b3-129">可以根据情况在请求正文中指定任何其他可写的 **messageRule** 属性。</span><span class="sxs-lookup"><span data-stu-id="404b3-129">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="404b3-130">参数</span><span class="sxs-lookup"><span data-stu-id="404b3-130">Parameter</span></span>       | <span data-ttu-id="404b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="404b3-131">Type</span></span>|<span data-ttu-id="404b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="404b3-132">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="404b3-133">actions</span><span class="sxs-lookup"><span data-stu-id="404b3-133">actions</span></span>|[<span data-ttu-id="404b3-134">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="404b3-134">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="404b3-135">满足相应条件（如果有的话）时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="404b3-135">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="404b3-136">必需。</span><span class="sxs-lookup"><span data-stu-id="404b3-136">Required.</span></span>|
|<span data-ttu-id="404b3-137">conditions</span><span class="sxs-lookup"><span data-stu-id="404b3-137">conditions</span></span>|[<span data-ttu-id="404b3-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="404b3-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="404b3-139">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="404b3-139">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="404b3-140">可选。</span><span class="sxs-lookup"><span data-stu-id="404b3-140">Optional.</span></span>|
|<span data-ttu-id="404b3-141">displayName</span><span class="sxs-lookup"><span data-stu-id="404b3-141">displayName</span></span>| <span data-ttu-id="404b3-142">String</span><span class="sxs-lookup"><span data-stu-id="404b3-142">String</span></span>  | <span data-ttu-id="404b3-143">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="404b3-143">The display name of the rule.</span></span> <span data-ttu-id="404b3-144">必需。</span><span class="sxs-lookup"><span data-stu-id="404b3-144">Required.</span></span>|
|<span data-ttu-id="404b3-145">exceptions</span><span class="sxs-lookup"><span data-stu-id="404b3-145">exceptions</span></span>| [<span data-ttu-id="404b3-146">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="404b3-146">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="404b3-147">表示规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="404b3-147">Represents exception conditions for the rule.</span></span> <span data-ttu-id="404b3-148">可选。</span><span class="sxs-lookup"><span data-stu-id="404b3-148">Optional.</span></span> |
|<span data-ttu-id="404b3-149">isEnabled</span><span class="sxs-lookup"><span data-stu-id="404b3-149">isEnabled</span></span> | <span data-ttu-id="404b3-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="404b3-150">Boolean</span></span> | <span data-ttu-id="404b3-151">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="404b3-151">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="404b3-152">可选。</span><span class="sxs-lookup"><span data-stu-id="404b3-152">Optional.</span></span> |
|<span data-ttu-id="404b3-153">Sequence</span><span class="sxs-lookup"><span data-stu-id="404b3-153">sequence</span></span>| <span data-ttu-id="404b3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="404b3-154">Int32</span></span> | <span data-ttu-id="404b3-155">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="404b3-155">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="404b3-156">必需。</span><span class="sxs-lookup"><span data-stu-id="404b3-156">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="404b3-157">响应</span><span class="sxs-lookup"><span data-stu-id="404b3-157">Response</span></span>
<span data-ttu-id="404b3-158">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="404b3-158">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="404b3-159">示例</span><span class="sxs-lookup"><span data-stu-id="404b3-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="404b3-160">请求</span><span class="sxs-lookup"><span data-stu-id="404b3-160">Request</span></span>
<span data-ttu-id="404b3-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="404b3-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="404b3-162">响应</span><span class="sxs-lookup"><span data-stu-id="404b3-162">Response</span></span>
<span data-ttu-id="404b3-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="404b3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
