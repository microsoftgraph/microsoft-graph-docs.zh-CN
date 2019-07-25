---
title: 获取 rule
description: 获取 messageRule 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7d606bc54f294263a03d99e804e3870f22d93a95
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879318"
---
# <a name="get-rule"></a><span data-ttu-id="273bb-103">获取 rule</span><span class="sxs-lookup"><span data-stu-id="273bb-103">Get rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="273bb-104">获取 [messageRule](../resources/messagerule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="273bb-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="273bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="273bb-105">Permissions</span></span>
<span data-ttu-id="273bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="273bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="273bb-108">Permission type</span></span>      | <span data-ttu-id="273bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="273bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="273bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="273bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="273bb-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="273bb-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="273bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="273bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="273bb-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="273bb-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="273bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="273bb-114">Application</span></span> | <span data-ttu-id="273bb-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="273bb-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="273bb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="273bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="273bb-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="273bb-117">Optional query parameters</span></span>
<span data-ttu-id="273bb-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="273bb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="273bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="273bb-119">Request headers</span></span>
| <span data-ttu-id="273bb-120">名称</span><span class="sxs-lookup"><span data-stu-id="273bb-120">Name</span></span>      |<span data-ttu-id="273bb-121">说明</span><span class="sxs-lookup"><span data-stu-id="273bb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="273bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="273bb-122">Authorization</span></span>  | <span data-ttu-id="273bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="273bb-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="273bb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="273bb-125">Request body</span></span>
<span data-ttu-id="273bb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="273bb-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="273bb-127">响应</span><span class="sxs-lookup"><span data-stu-id="273bb-127">Response</span></span>
<span data-ttu-id="273bb-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="273bb-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="273bb-129">示例</span><span class="sxs-lookup"><span data-stu-id="273bb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="273bb-130">请求</span><span class="sxs-lookup"><span data-stu-id="273bb-130">Request</span></span>
<span data-ttu-id="273bb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="273bb-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="273bb-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="273bb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="273bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="273bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="273bb-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="273bb-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="273bb-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="273bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="273bb-136">Java</span><span class="sxs-lookup"><span data-stu-id="273bb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="273bb-137">响应</span><span class="sxs-lookup"><span data-stu-id="273bb-137">Response</span></span>
<span data-ttu-id="273bb-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="273bb-138">Here is an example of the response.</span></span> <span data-ttu-id="273bb-139">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="273bb-139">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="273bb-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="273bb-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
