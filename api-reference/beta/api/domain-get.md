---
title: 获取 domain
description: 检索 domain 对象的属性和关系。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 49458b87f86bc5a7dbf4d7d3c196736050b2d6aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813571"
---
# <a name="get-domain"></a><span data-ttu-id="608b4-103">获取 domain</span><span class="sxs-lookup"><span data-stu-id="608b4-103">Get domain</span></span>

> <span data-ttu-id="608b4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="608b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="608b4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="608b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="608b4-106">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="608b4-106">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="608b4-107">权限</span><span class="sxs-lookup"><span data-stu-id="608b4-107">Permissions</span></span>

<span data-ttu-id="608b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="608b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="608b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="608b4-110">Permission type</span></span>      | <span data-ttu-id="608b4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="608b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="608b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="608b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="608b4-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="608b4-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="608b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="608b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="608b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="608b4-115">Not supported.</span></span>    |
|<span data-ttu-id="608b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="608b4-116">Application</span></span> | <span data-ttu-id="608b4-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="608b4-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="608b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="608b4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="608b4-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="608b4-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="608b4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="608b4-120">Optional query parameters</span></span>

<span data-ttu-id="608b4-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="608b4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="608b4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="608b4-122">Request headers</span></span>

| <span data-ttu-id="608b4-123">名称</span><span class="sxs-lookup"><span data-stu-id="608b4-123">Name</span></span>      |<span data-ttu-id="608b4-124">说明</span><span class="sxs-lookup"><span data-stu-id="608b4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="608b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="608b4-125">Authorization</span></span>  | <span data-ttu-id="608b4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="608b4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="608b4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="608b4-128">Content-Type</span></span>  | <span data-ttu-id="608b4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="608b4-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="608b4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="608b4-130">Request body</span></span>
<span data-ttu-id="608b4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="608b4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="608b4-132">响应</span><span class="sxs-lookup"><span data-stu-id="608b4-132">Response</span></span>

<span data-ttu-id="608b4-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="608b4-133">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="608b4-134">示例</span><span class="sxs-lookup"><span data-stu-id="608b4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="608b4-135">请求</span><span class="sxs-lookup"><span data-stu-id="608b4-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="608b4-136">响应</span><span class="sxs-lookup"><span data-stu-id="608b4-136">Response</span></span>
<span data-ttu-id="608b4-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="608b4-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
