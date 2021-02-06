---
title: 列出规则
description: 获取为用户的收件箱定义的所有 messageRule 对象。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 84cc52dd989d8534aa09319cfcbdffe75adffad9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131234"
---
# <a name="list-rules"></a><span data-ttu-id="74784-103">列出规则</span><span class="sxs-lookup"><span data-stu-id="74784-103">List rules</span></span>

<span data-ttu-id="74784-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74784-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74784-105">获取为用户收件箱定义的所有 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74784-105">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="74784-106">权限</span><span class="sxs-lookup"><span data-stu-id="74784-106">Permissions</span></span>
<span data-ttu-id="74784-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74784-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="74784-109">Permission type</span></span>      | <span data-ttu-id="74784-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74784-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74784-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74784-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74784-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="74784-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="74784-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74784-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74784-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="74784-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="74784-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="74784-115">Application</span></span> | <span data-ttu-id="74784-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="74784-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="74784-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74784-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74784-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="74784-118">Optional query parameters</span></span>
<span data-ttu-id="74784-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="74784-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="74784-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74784-120">Request headers</span></span>
| <span data-ttu-id="74784-121">名称</span><span class="sxs-lookup"><span data-stu-id="74784-121">Name</span></span>       | <span data-ttu-id="74784-122">类型</span><span class="sxs-lookup"><span data-stu-id="74784-122">Type</span></span> | <span data-ttu-id="74784-123">说明</span><span class="sxs-lookup"><span data-stu-id="74784-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74784-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="74784-124">Authorization</span></span>  | <span data-ttu-id="74784-125">string</span><span class="sxs-lookup"><span data-stu-id="74784-125">string</span></span>  | <span data-ttu-id="74784-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74784-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74784-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="74784-128">Request body</span></span>
<span data-ttu-id="74784-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74784-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="74784-130">响应</span><span class="sxs-lookup"><span data-stu-id="74784-130">Response</span></span>
<span data-ttu-id="74784-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="74784-131">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74784-132">示例</span><span class="sxs-lookup"><span data-stu-id="74784-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74784-133">请求</span><span class="sxs-lookup"><span data-stu-id="74784-133">Request</span></span>
<span data-ttu-id="74784-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74784-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74784-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="74784-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
# <a name="c"></a>[<span data-ttu-id="74784-136">C#</span><span class="sxs-lookup"><span data-stu-id="74784-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74784-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74784-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74784-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74784-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74784-139">Java</span><span class="sxs-lookup"><span data-stu-id="74784-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="74784-140">响应</span><span class="sxs-lookup"><span data-stu-id="74784-140">Response</span></span>
<span data-ttu-id="74784-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74784-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
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
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
