---
title: 获取 rule
description: 获取 messageRule 对象的属性和关系。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8e766ab2b3a7c59ccb8a6195da95356a44fb6b10
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981020"
---
# <a name="get-rule"></a><span data-ttu-id="75cbb-103">获取规则</span><span class="sxs-lookup"><span data-stu-id="75cbb-103">Get rule</span></span>

<span data-ttu-id="75cbb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75cbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75cbb-105">获取 [messageRule](../resources/messagerule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75cbb-105">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="75cbb-106">权限</span><span class="sxs-lookup"><span data-stu-id="75cbb-106">Permissions</span></span>
<span data-ttu-id="75cbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75cbb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="75cbb-109">Permission type</span></span>      | <span data-ttu-id="75cbb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75cbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75cbb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75cbb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75cbb-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="75cbb-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="75cbb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75cbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75cbb-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="75cbb-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="75cbb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="75cbb-115">Application</span></span> | <span data-ttu-id="75cbb-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="75cbb-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="75cbb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75cbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="75cbb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75cbb-118">Optional query parameters</span></span>
<span data-ttu-id="75cbb-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75cbb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75cbb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="75cbb-120">Request headers</span></span>
| <span data-ttu-id="75cbb-121">名称</span><span class="sxs-lookup"><span data-stu-id="75cbb-121">Name</span></span>      |<span data-ttu-id="75cbb-122">说明</span><span class="sxs-lookup"><span data-stu-id="75cbb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75cbb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75cbb-123">Authorization</span></span>  | <span data-ttu-id="75cbb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75cbb-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="75cbb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="75cbb-126">Request body</span></span>
<span data-ttu-id="75cbb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75cbb-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="75cbb-128">响应</span><span class="sxs-lookup"><span data-stu-id="75cbb-128">Response</span></span>
<span data-ttu-id="75cbb-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75cbb-129">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75cbb-130">示例</span><span class="sxs-lookup"><span data-stu-id="75cbb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75cbb-131">请求</span><span class="sxs-lookup"><span data-stu-id="75cbb-131">Request</span></span>
<span data-ttu-id="75cbb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75cbb-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75cbb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="75cbb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
# <a name="c"></a>[<span data-ttu-id="75cbb-134">C#</span><span class="sxs-lookup"><span data-stu-id="75cbb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75cbb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75cbb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75cbb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75cbb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75cbb-137">Java</span><span class="sxs-lookup"><span data-stu-id="75cbb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75cbb-138">响应</span><span class="sxs-lookup"><span data-stu-id="75cbb-138">Response</span></span>
<span data-ttu-id="75cbb-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="75cbb-139">Here is an example of the response.</span></span> <span data-ttu-id="75cbb-140">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="75cbb-140">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="75cbb-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75cbb-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
