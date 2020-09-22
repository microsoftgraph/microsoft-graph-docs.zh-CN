---
title: 列出 subscribedSkus
description: 检索组织已获取的商业订阅列表。
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ad3e5c16de0462127589b99c14a498cb2bbc005
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044352"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="7ba19-103">列出 subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="7ba19-103">List subscribedSkus</span></span>

<span data-ttu-id="7ba19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ba19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba19-105">获取组织已获取的商业版订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="7ba19-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ba19-106">权限</span><span class="sxs-lookup"><span data-stu-id="7ba19-106">Permissions</span></span>
<span data-ttu-id="7ba19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ba19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ba19-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ba19-109">Permission type</span></span>      | <span data-ttu-id="7ba19-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ba19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ba19-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ba19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ba19-112">全部、全部、全部、Directory.accessasuser.all、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="7ba19-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ba19-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ba19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ba19-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ba19-114">Not supported.</span></span>    |
|<span data-ttu-id="7ba19-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ba19-115">Application</span></span> | <span data-ttu-id="7ba19-116">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ba19-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ba19-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ba19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ba19-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7ba19-118">Optional query parameters</span></span>

<span data-ttu-id="7ba19-119">此方法不支持 [OData 查询参数](/graph//query-parameters) ，以帮助自定义不支持的响应 (`$filter`) 。</span><span class="sxs-lookup"><span data-stu-id="7ba19-119">This method does not support the [OData query parameters](/graph//query-parameters) to help customize the response (`$filter` is not supported).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ba19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ba19-120">Request headers</span></span>

| <span data-ttu-id="7ba19-121">名称</span><span class="sxs-lookup"><span data-stu-id="7ba19-121">Name</span></span>       | <span data-ttu-id="7ba19-122">说明</span><span class="sxs-lookup"><span data-stu-id="7ba19-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7ba19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ba19-123">Authorization</span></span>  | <span data-ttu-id="7ba19-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ba19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ba19-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ba19-126">Request body</span></span>
<span data-ttu-id="7ba19-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ba19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ba19-128">响应</span><span class="sxs-lookup"><span data-stu-id="7ba19-128">Response</span></span>

<span data-ttu-id="7ba19-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7ba19-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ba19-130">示例</span><span class="sxs-lookup"><span data-stu-id="7ba19-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ba19-131">请求</span><span class="sxs-lookup"><span data-stu-id="7ba19-131">Request</span></span>
<span data-ttu-id="7ba19-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ba19-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ba19-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ba19-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="7ba19-134">C#</span><span class="sxs-lookup"><span data-stu-id="7ba19-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ba19-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ba19-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ba19-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ba19-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7ba19-137">响应</span><span class="sxs-lookup"><span data-stu-id="7ba19-137">Response</span></span>
<span data-ttu-id="7ba19-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ba19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


