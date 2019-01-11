---
title: 列表 agreementAcceptances
description: 检索用户的 agreementAcceptance 对象的列表。
localization_priority: Normal
ms.openlocfilehash: ed0f93f7b0aac2ff0cbaf9a318bfc571261147bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879735"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="235a3-103">列表 agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="235a3-103">List agreementAcceptances</span></span>

> <span data-ttu-id="235a3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="235a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="235a3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="235a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="235a3-106">检索用户的[agreementAcceptance](../resources/agreementacceptance.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="235a3-106">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="235a3-107">权限</span><span class="sxs-lookup"><span data-stu-id="235a3-107">Permissions</span></span>
<span data-ttu-id="235a3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="235a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="235a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="235a3-110">Permission type</span></span>                        | <span data-ttu-id="235a3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="235a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="235a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="235a3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="235a3-113">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="235a3-113">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="235a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="235a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="235a3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="235a3-115">Not supported.</span></span> |
|<span data-ttu-id="235a3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="235a3-116">Application</span></span>                            | <span data-ttu-id="235a3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="235a3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="235a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="235a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="235a3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="235a3-119">Request headers</span></span>
| <span data-ttu-id="235a3-120">名称</span><span class="sxs-lookup"><span data-stu-id="235a3-120">Name</span></span>      |<span data-ttu-id="235a3-121">说明</span><span class="sxs-lookup"><span data-stu-id="235a3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="235a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="235a3-122">Authorization</span></span> | <span data-ttu-id="235a3-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="235a3-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="235a3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="235a3-124">Request body</span></span>
<span data-ttu-id="235a3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="235a3-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="235a3-126">响应</span><span class="sxs-lookup"><span data-stu-id="235a3-126">Response</span></span>
<span data-ttu-id="235a3-127">如果成功，此方法返回`200 OK`响应代码和响应正文中的[agreementAcceptance](../resources/agreementacceptance.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="235a3-127">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="235a3-128">示例</span><span class="sxs-lookup"><span data-stu-id="235a3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="235a3-129">请求</span><span class="sxs-lookup"><span data-stu-id="235a3-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="235a3-130">响应</span><span class="sxs-lookup"><span data-stu-id="235a3-130">Response</span></span>
><span data-ttu-id="235a3-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="235a3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
