---
title: 列表协议
description: 检索协议对象的列表。
localization_priority: Normal
ms.openlocfilehash: 3ae255a386986b5627aed99f29dca5bfb9934e30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859918"
---
# <a name="list-agreements"></a><span data-ttu-id="de4a2-103">列表协议</span><span class="sxs-lookup"><span data-stu-id="de4a2-103">List agreements</span></span>

> <span data-ttu-id="de4a2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de4a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de4a2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de4a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de4a2-106">检索[协议](../resources/agreement.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="de4a2-106">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="de4a2-107">权限</span><span class="sxs-lookup"><span data-stu-id="de4a2-107">Permissions</span></span>
<span data-ttu-id="de4a2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de4a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de4a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de4a2-110">Permission type</span></span>                        | <span data-ttu-id="de4a2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de4a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="de4a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de4a2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="de4a2-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="de4a2-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="de4a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de4a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de4a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de4a2-115">Not supported.</span></span> |
|<span data-ttu-id="de4a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de4a2-116">Application</span></span>                            | <span data-ttu-id="de4a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="de4a2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de4a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de4a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="de4a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="de4a2-119">Request headers</span></span>
| <span data-ttu-id="de4a2-120">名称</span><span class="sxs-lookup"><span data-stu-id="de4a2-120">Name</span></span>         | <span data-ttu-id="de4a2-121">类型</span><span class="sxs-lookup"><span data-stu-id="de4a2-121">Type</span></span>        | <span data-ttu-id="de4a2-122">说明</span><span class="sxs-lookup"><span data-stu-id="de4a2-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="de4a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de4a2-123">Authorization</span></span> | <span data-ttu-id="de4a2-124">string</span><span class="sxs-lookup"><span data-stu-id="de4a2-124">string</span></span> | <span data-ttu-id="de4a2-125">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="de4a2-125">Bearer \{token\}.</span></span> <span data-ttu-id="de4a2-126">必填。</span><span class="sxs-lookup"><span data-stu-id="de4a2-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de4a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de4a2-127">Request body</span></span>
<span data-ttu-id="de4a2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de4a2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="de4a2-129">响应</span><span class="sxs-lookup"><span data-stu-id="de4a2-129">Response</span></span>
<span data-ttu-id="de4a2-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[协议](../resources/agreement.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="de4a2-130">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de4a2-131">示例</span><span class="sxs-lookup"><span data-stu-id="de4a2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de4a2-132">请求</span><span class="sxs-lookup"><span data-stu-id="de4a2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="de4a2-133">响应</span><span class="sxs-lookup"><span data-stu-id="de4a2-133">Response</span></span>
><span data-ttu-id="de4a2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="de4a2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
