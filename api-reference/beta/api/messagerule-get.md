---
title: 获取 rule
description: 获取 messageRule 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 06d824e8cb761b4ffadc0b95284cdfb5326a285b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597901"
---
# <a name="get-rule"></a><span data-ttu-id="17fd3-103">获取 rule</span><span class="sxs-lookup"><span data-stu-id="17fd3-103">Get rule</span></span>


<span data-ttu-id="17fd3-104">获取 [messageRule](../resources/messagerule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17fd3-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="17fd3-105">权限</span><span class="sxs-lookup"><span data-stu-id="17fd3-105">Permissions</span></span>
<span data-ttu-id="17fd3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17fd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17fd3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="17fd3-108">Permission type</span></span>      | <span data-ttu-id="17fd3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17fd3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17fd3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17fd3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17fd3-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="17fd3-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="17fd3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17fd3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17fd3-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="17fd3-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="17fd3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="17fd3-114">Application</span></span> | <span data-ttu-id="17fd3-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="17fd3-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="17fd3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17fd3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17fd3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17fd3-117">Optional query parameters</span></span>
<span data-ttu-id="17fd3-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="17fd3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17fd3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="17fd3-119">Request headers</span></span>
| <span data-ttu-id="17fd3-120">名称</span><span class="sxs-lookup"><span data-stu-id="17fd3-120">Name</span></span>      |<span data-ttu-id="17fd3-121">说明</span><span class="sxs-lookup"><span data-stu-id="17fd3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17fd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17fd3-122">Authorization</span></span>  | <span data-ttu-id="17fd3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17fd3-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="17fd3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="17fd3-125">Request body</span></span>
<span data-ttu-id="17fd3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17fd3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="17fd3-127">响应</span><span class="sxs-lookup"><span data-stu-id="17fd3-127">Response</span></span>
<span data-ttu-id="17fd3-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17fd3-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17fd3-129">示例</span><span class="sxs-lookup"><span data-stu-id="17fd3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17fd3-130">请求</span><span class="sxs-lookup"><span data-stu-id="17fd3-130">Request</span></span>
<span data-ttu-id="17fd3-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17fd3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="17fd3-132">响应</span><span class="sxs-lookup"><span data-stu-id="17fd3-132">Response</span></span>
<span data-ttu-id="17fd3-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="17fd3-133">Here is an example of the response.</span></span> <span data-ttu-id="17fd3-134">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="17fd3-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="17fd3-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17fd3-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="17fd3-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="17fd3-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="17fd3-138">语言</span><span class="sxs-lookup"><span data-stu-id="17fd3-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messagerule-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17fd3-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="17fd3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messagerule-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
