---
title: 获取 rule
description: 获取 messageRule 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 45fe9ccf24777a74b55d2934a34ba7d1c571fb0e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449314"
---
# <a name="get-rule"></a><span data-ttu-id="4e11c-103">获取 rule</span><span class="sxs-lookup"><span data-stu-id="4e11c-103">Get rule</span></span>


<span data-ttu-id="4e11c-104">获取 [messageRule](../resources/messagerule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4e11c-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="4e11c-105">权限</span><span class="sxs-lookup"><span data-stu-id="4e11c-105">Permissions</span></span>
<span data-ttu-id="4e11c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e11c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e11c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e11c-108">Permission type</span></span>      | <span data-ttu-id="4e11c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e11c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e11c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e11c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e11c-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4e11c-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4e11c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e11c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e11c-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4e11c-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4e11c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e11c-114">Application</span></span> | <span data-ttu-id="4e11c-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4e11c-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e11c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e11c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4e11c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4e11c-117">Optional query parameters</span></span>
<span data-ttu-id="4e11c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4e11c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e11c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e11c-119">Request headers</span></span>
| <span data-ttu-id="4e11c-120">名称</span><span class="sxs-lookup"><span data-stu-id="4e11c-120">Name</span></span>      |<span data-ttu-id="4e11c-121">说明</span><span class="sxs-lookup"><span data-stu-id="4e11c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e11c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e11c-122">Authorization</span></span>  | <span data-ttu-id="4e11c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e11c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4e11c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e11c-125">Request body</span></span>
<span data-ttu-id="4e11c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e11c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e11c-127">响应</span><span class="sxs-lookup"><span data-stu-id="4e11c-127">Response</span></span>
<span data-ttu-id="4e11c-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e11c-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e11c-129">示例</span><span class="sxs-lookup"><span data-stu-id="4e11c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e11c-130">请求</span><span class="sxs-lookup"><span data-stu-id="4e11c-130">Request</span></span>
<span data-ttu-id="4e11c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e11c-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e11c-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4e11c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e11c-133">C#</span><span class="sxs-lookup"><span data-stu-id="4e11c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e11c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="4e11c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e11c-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="4e11c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e11c-136">响应</span><span class="sxs-lookup"><span data-stu-id="4e11c-136">Response</span></span>
<span data-ttu-id="4e11c-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e11c-137">Here is an example of the response.</span></span> <span data-ttu-id="4e11c-138">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="4e11c-138">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="4e11c-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e11c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
