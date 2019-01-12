---
title: 列出组织
description: 检索 organization 对象列表。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9dd1489714c4de87f0072ef0498c5acdf008d5ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938823"
---
# <a name="list-organization"></a><span data-ttu-id="2558c-103">列出组织</span><span class="sxs-lookup"><span data-stu-id="2558c-103">List organization</span></span>

> <span data-ttu-id="2558c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2558c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2558c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2558c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2558c-106">检索组织对象列表。</span><span class="sxs-lookup"><span data-stu-id="2558c-106">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2558c-107">权限</span><span class="sxs-lookup"><span data-stu-id="2558c-107">Permissions</span></span>
<span data-ttu-id="2558c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2558c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2558c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2558c-110">Permission type</span></span>      | <span data-ttu-id="2558c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2558c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2558c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2558c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2558c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2558c-113">Not supported.</span></span>    |
|<span data-ttu-id="2558c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2558c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2558c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2558c-115">Not supported.</span></span>    |
|<span data-ttu-id="2558c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2558c-116">Application</span></span> | <span data-ttu-id="2558c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2558c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2558c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2558c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2558c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2558c-119">Optional query parameters</span></span>
<span data-ttu-id="2558c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2558c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2558c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2558c-121">Request headers</span></span>
| <span data-ttu-id="2558c-122">名称</span><span class="sxs-lookup"><span data-stu-id="2558c-122">Name</span></span>       | <span data-ttu-id="2558c-123">类型</span><span class="sxs-lookup"><span data-stu-id="2558c-123">Type</span></span> | <span data-ttu-id="2558c-124">说明</span><span class="sxs-lookup"><span data-stu-id="2558c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2558c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2558c-125">Authorization</span></span>  | <span data-ttu-id="2558c-126">string</span><span class="sxs-lookup"><span data-stu-id="2558c-126">string</span></span>  | <span data-ttu-id="2558c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2558c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2558c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2558c-129">Request body</span></span>
<span data-ttu-id="2558c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2558c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2558c-131">响应</span><span class="sxs-lookup"><span data-stu-id="2558c-131">Response</span></span>

<span data-ttu-id="2558c-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2558c-132">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2558c-133">示例</span><span class="sxs-lookup"><span data-stu-id="2558c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2558c-134">请求</span><span class="sxs-lookup"><span data-stu-id="2558c-134">Request</span></span>
<span data-ttu-id="2558c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2558c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="2558c-136">响应</span><span class="sxs-lookup"><span data-stu-id="2558c-136">Response</span></span>
<span data-ttu-id="2558c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2558c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
