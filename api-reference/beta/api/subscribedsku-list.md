---
title: 列出 subscribedSkus
description: 检索组织已获取的商业订阅列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 715ff4ac14d8652f4a6f1e9cc87e5e10173cea2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991189"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="4373b-103">列出 subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="4373b-103">List subscribedSkus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4373b-104">获取组织获取的商业订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="4373b-104">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="4373b-105">权限</span><span class="sxs-lookup"><span data-stu-id="4373b-105">Permissions</span></span>
<span data-ttu-id="4373b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4373b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4373b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4373b-108">Permission type</span></span>      | <span data-ttu-id="4373b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4373b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4373b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4373b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4373b-111">全部、全部、全部、Directory.accessasuser.all、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="4373b-111">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4373b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4373b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4373b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4373b-113">Not supported.</span></span>    |
|<span data-ttu-id="4373b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4373b-114">Application</span></span> | <span data-ttu-id="4373b-115">全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="4373b-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4373b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4373b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4373b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4373b-117">Optional query parameters</span></span>
<span data-ttu-id="4373b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4373b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4373b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4373b-119">Request headers</span></span>

| <span data-ttu-id="4373b-120">名称</span><span class="sxs-lookup"><span data-stu-id="4373b-120">Name</span></span>       | <span data-ttu-id="4373b-121">说明</span><span class="sxs-lookup"><span data-stu-id="4373b-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4373b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4373b-122">Authorization</span></span>  | <span data-ttu-id="4373b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4373b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4373b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4373b-125">Request body</span></span>
<span data-ttu-id="4373b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4373b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4373b-127">响应</span><span class="sxs-lookup"><span data-stu-id="4373b-127">Response</span></span>

<span data-ttu-id="4373b-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4373b-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4373b-129">示例</span><span class="sxs-lookup"><span data-stu-id="4373b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4373b-130">请求</span><span class="sxs-lookup"><span data-stu-id="4373b-130">Request</span></span>
<span data-ttu-id="4373b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4373b-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4373b-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4373b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4373b-133">C#</span><span class="sxs-lookup"><span data-stu-id="4373b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4373b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="4373b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4373b-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="4373b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4373b-136">Java</span><span class="sxs-lookup"><span data-stu-id="4373b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4373b-137">响应</span><span class="sxs-lookup"><span data-stu-id="4373b-137">Response</span></span>
<span data-ttu-id="4373b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4373b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
