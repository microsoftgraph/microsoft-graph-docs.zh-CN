---
title: 获取 rule
description: 获取 messageRule 对象的属性和关系。
ms.openlocfilehash: 0151a83f54c67e6daf5c78766f6d4a532108bfda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048775"
---
# <a name="get-rule"></a><span data-ttu-id="d2a0a-103">获取 rule</span><span class="sxs-lookup"><span data-stu-id="d2a0a-103">Get rule</span></span>

> <span data-ttu-id="d2a0a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2a0a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2a0a-106">获取 [messageRule](../resources/messagerule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-106">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="d2a0a-107">权限</span><span class="sxs-lookup"><span data-stu-id="d2a0a-107">Permissions</span></span>
<span data-ttu-id="d2a0a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2a0a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2a0a-110">Permission type</span></span>      | <span data-ttu-id="d2a0a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2a0a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2a0a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2a0a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2a0a-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d2a0a-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d2a0a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2a0a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2a0a-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d2a0a-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d2a0a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2a0a-116">Application</span></span> | <span data-ttu-id="d2a0a-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d2a0a-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2a0a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2a0a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2a0a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d2a0a-119">Optional query parameters</span></span>
<span data-ttu-id="d2a0a-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2a0a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2a0a-121">Request headers</span></span>
| <span data-ttu-id="d2a0a-122">名称</span><span class="sxs-lookup"><span data-stu-id="d2a0a-122">Name</span></span>      |<span data-ttu-id="d2a0a-123">说明</span><span class="sxs-lookup"><span data-stu-id="d2a0a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2a0a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2a0a-124">Authorization</span></span>  | <span data-ttu-id="d2a0a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d2a0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2a0a-127">Request body</span></span>
<span data-ttu-id="d2a0a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2a0a-129">响应</span><span class="sxs-lookup"><span data-stu-id="d2a0a-129">Response</span></span>
<span data-ttu-id="d2a0a-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-130">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2a0a-131">示例</span><span class="sxs-lookup"><span data-stu-id="d2a0a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2a0a-132">请求</span><span class="sxs-lookup"><span data-stu-id="d2a0a-132">Request</span></span>
<span data-ttu-id="d2a0a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="d2a0a-134">响应</span><span class="sxs-lookup"><span data-stu-id="d2a0a-134">Response</span></span>
<span data-ttu-id="d2a0a-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-135">Here is an example of the response.</span></span> <span data-ttu-id="d2a0a-136">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-136">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="d2a0a-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2a0a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->