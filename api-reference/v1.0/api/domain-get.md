---
title: 获取域
description: 检索 domain 对象的属性和关系。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93139514ae66b4af4c6ade8de8f068050b985451
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467209"
---
# <a name="get-domain"></a><span data-ttu-id="8606d-103">获取域</span><span class="sxs-lookup"><span data-stu-id="8606d-103">Get domain</span></span>

<span data-ttu-id="8606d-104">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8606d-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8606d-105">权限</span><span class="sxs-lookup"><span data-stu-id="8606d-105">Permissions</span></span>

<span data-ttu-id="8606d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8606d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8606d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8606d-108">Permission type</span></span>      | <span data-ttu-id="8606d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8606d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8606d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8606d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8606d-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8606d-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="8606d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8606d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8606d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8606d-113">Not supported.</span></span>    |
|<span data-ttu-id="8606d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8606d-114">Application</span></span> | <span data-ttu-id="8606d-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8606d-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8606d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8606d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="8606d-117">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="8606d-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8606d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8606d-118">Optional query parameters</span></span>

<span data-ttu-id="8606d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8606d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8606d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8606d-120">Request headers</span></span>

| <span data-ttu-id="8606d-121">名称</span><span class="sxs-lookup"><span data-stu-id="8606d-121">Name</span></span>      |<span data-ttu-id="8606d-122">说明</span><span class="sxs-lookup"><span data-stu-id="8606d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8606d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8606d-123">Authorization</span></span>  | <span data-ttu-id="8606d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8606d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8606d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8606d-126">Content-Type</span></span>  | <span data-ttu-id="8606d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8606d-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8606d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8606d-128">Request body</span></span>
<span data-ttu-id="8606d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8606d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8606d-130">响应</span><span class="sxs-lookup"><span data-stu-id="8606d-130">Response</span></span>

<span data-ttu-id="8606d-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[domain](../resources/domain.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8606d-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8606d-132">示例</span><span class="sxs-lookup"><span data-stu-id="8606d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8606d-133">请求</span><span class="sxs-lookup"><span data-stu-id="8606d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="8606d-134">响应</span><span class="sxs-lookup"><span data-stu-id="8606d-134">Response</span></span>
<span data-ttu-id="8606d-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8606d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
