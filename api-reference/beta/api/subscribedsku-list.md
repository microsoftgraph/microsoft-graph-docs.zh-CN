---
title: 列出 subscribedSkus
description: 检索组织已获取的商业订阅列表。
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 416f91448a8bba9852f68bb5587818555ee4ca78
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048965"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="189f7-103">列出 subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="189f7-103">List subscribedSkus</span></span>

<span data-ttu-id="189f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="189f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="189f7-105">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="189f7-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="189f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="189f7-106">Permissions</span></span>
<span data-ttu-id="189f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="189f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="189f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="189f7-109">Permission type</span></span>      | <span data-ttu-id="189f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="189f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="189f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="189f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="189f7-112">Organization.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="189f7-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="189f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="189f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="189f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="189f7-114">Not supported.</span></span>    |
|<span data-ttu-id="189f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="189f7-115">Application</span></span> | <span data-ttu-id="189f7-116">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189f7-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="189f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="189f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="189f7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="189f7-118">Optional query parameters</span></span>

<span data-ttu-id="189f7-119">此方法不支持 [OData 查询](/graph//query-parameters) 参数来帮助自定义响应 (`$filter` 不支持) 。</span><span class="sxs-lookup"><span data-stu-id="189f7-119">This method does not support the [OData query parameters](/graph//query-parameters) to help customize the response (`$filter` is not supported).</span></span>

## <a name="request-headers"></a><span data-ttu-id="189f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="189f7-120">Request headers</span></span>

| <span data-ttu-id="189f7-121">名称</span><span class="sxs-lookup"><span data-stu-id="189f7-121">Name</span></span>       | <span data-ttu-id="189f7-122">说明</span><span class="sxs-lookup"><span data-stu-id="189f7-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="189f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="189f7-123">Authorization</span></span>  | <span data-ttu-id="189f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="189f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="189f7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="189f7-126">Request body</span></span>
<span data-ttu-id="189f7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="189f7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="189f7-128">响应</span><span class="sxs-lookup"><span data-stu-id="189f7-128">Response</span></span>

<span data-ttu-id="189f7-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="189f7-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="189f7-130">示例</span><span class="sxs-lookup"><span data-stu-id="189f7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="189f7-131">请求</span><span class="sxs-lookup"><span data-stu-id="189f7-131">Request</span></span>
<span data-ttu-id="189f7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="189f7-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="189f7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="189f7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="189f7-134">C#</span><span class="sxs-lookup"><span data-stu-id="189f7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="189f7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="189f7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="189f7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="189f7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="189f7-137">Java</span><span class="sxs-lookup"><span data-stu-id="189f7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="189f7-138">响应</span><span class="sxs-lookup"><span data-stu-id="189f7-138">Response</span></span>
<span data-ttu-id="189f7-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="189f7-139">Here is an example of the response.</span></span> <span data-ttu-id="189f7-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="189f7-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
  "value": [
    {
      "capabilityStatus": "capabilityStatus-value",
      "consumedUnits": 99,
      "prepaidUnits": {
        "enabled": 99,
        "suspended": 99,
        "warning": 99
      },
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


