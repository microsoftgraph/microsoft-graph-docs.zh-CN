---
title: 获取 domain
description: 检索 domain 对象的属性和关系。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 4d49fe39f9e953b6e0bcdb4504a4f2296d5d4ff9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817218"
---
# <a name="get-domain"></a><span data-ttu-id="ad584-103">获取 domain</span><span class="sxs-lookup"><span data-stu-id="ad584-103">Get domain</span></span>

<span data-ttu-id="ad584-104">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad584-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad584-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad584-105">Permissions</span></span>

<span data-ttu-id="ad584-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad584-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad584-108">Permission type</span></span>      | <span data-ttu-id="ad584-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad584-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad584-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad584-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad584-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad584-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="ad584-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad584-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad584-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad584-113">Not supported.</span></span>    |
|<span data-ttu-id="ad584-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad584-114">Application</span></span> | <span data-ttu-id="ad584-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad584-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad584-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad584-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="ad584-117">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="ad584-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ad584-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ad584-118">Optional query parameters</span></span>

<span data-ttu-id="ad584-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad584-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad584-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad584-120">Request headers</span></span>

| <span data-ttu-id="ad584-121">名称</span><span class="sxs-lookup"><span data-stu-id="ad584-121">Name</span></span>      |<span data-ttu-id="ad584-122">说明</span><span class="sxs-lookup"><span data-stu-id="ad584-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad584-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad584-123">Authorization</span></span>  | <span data-ttu-id="ad584-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad584-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad584-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad584-126">Content-Type</span></span>  | <span data-ttu-id="ad584-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ad584-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad584-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad584-128">Request body</span></span>
<span data-ttu-id="ad584-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad584-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad584-130">响应</span><span class="sxs-lookup"><span data-stu-id="ad584-130">Response</span></span>

<span data-ttu-id="ad584-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad584-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad584-132">示例</span><span class="sxs-lookup"><span data-stu-id="ad584-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad584-133">请求</span><span class="sxs-lookup"><span data-stu-id="ad584-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="ad584-134">响应</span><span class="sxs-lookup"><span data-stu-id="ad584-134">Response</span></span>
<span data-ttu-id="ad584-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad584-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
