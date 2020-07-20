---
title: 获取 externalItem
description: 获取 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 0e668c6ee1d571287304e0920a4636c81cd06ca7
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45005137"
---
# <a name="get-externalitem"></a><span data-ttu-id="3be39-103">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="3be39-103">Get externalItem</span></span>

<span data-ttu-id="3be39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be39-105">获取[externalitem](../resources/externalitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3be39-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="3be39-106">此 API 是为诊断目的而提供的。</span><span class="sxs-lookup"><span data-stu-id="3be39-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="3be39-107">不应将其用于任何其他用途。</span><span class="sxs-lookup"><span data-stu-id="3be39-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="3be39-108">对此 API 的重复请求可能会导致 `429` 出现 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="3be39-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="3be39-109">权限</span><span class="sxs-lookup"><span data-stu-id="3be39-109">Permissions</span></span>

<span data-ttu-id="3be39-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3be39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3be39-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3be39-112">Permission type</span></span>                        | <span data-ttu-id="3be39-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3be39-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3be39-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3be39-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3be39-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3be39-115">Not supported.</span></span> |
| <span data-ttu-id="3be39-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3be39-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3be39-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3be39-117">Not supported.</span></span> |
| <span data-ttu-id="3be39-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3be39-118">Application</span></span>                            | <span data-ttu-id="3be39-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be39-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3be39-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3be39-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="3be39-121">路径参数</span><span class="sxs-lookup"><span data-stu-id="3be39-121">Path parameters</span></span>

| <span data-ttu-id="3be39-122">参数</span><span class="sxs-lookup"><span data-stu-id="3be39-122">Parameter</span></span>     | <span data-ttu-id="3be39-123">类型</span><span class="sxs-lookup"><span data-stu-id="3be39-123">Type</span></span>   | <span data-ttu-id="3be39-124">说明</span><span class="sxs-lookup"><span data-stu-id="3be39-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="3be39-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="3be39-125">connection-id</span></span> | <span data-ttu-id="3be39-126">string</span><span class="sxs-lookup"><span data-stu-id="3be39-126">string</span></span> | <span data-ttu-id="3be39-127">`id`包含[externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="3be39-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="3be39-128">item-id</span><span class="sxs-lookup"><span data-stu-id="3be39-128">item-id</span></span>       | <span data-ttu-id="3be39-129">string</span><span class="sxs-lookup"><span data-stu-id="3be39-129">string</span></span> | <span data-ttu-id="3be39-130">ExternalItem 的开发人员提供的 `id` 属性[externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3be39-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3be39-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3be39-131">Optional query parameters</span></span>

<span data-ttu-id="3be39-132">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="3be39-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3be39-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="3be39-133">Request headers</span></span>

| <span data-ttu-id="3be39-134">名称</span><span class="sxs-lookup"><span data-stu-id="3be39-134">Name</span></span>          | <span data-ttu-id="3be39-135">说明</span><span class="sxs-lookup"><span data-stu-id="3be39-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3be39-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="3be39-136">Authorization</span></span> | <span data-ttu-id="3be39-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3be39-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3be39-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="3be39-139">Request body</span></span>

<span data-ttu-id="3be39-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3be39-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3be39-141">响应</span><span class="sxs-lookup"><span data-stu-id="3be39-141">Response</span></span>

<span data-ttu-id="3be39-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[externalItem](../resources/externalitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3be39-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be39-143">示例</span><span class="sxs-lookup"><span data-stu-id="3be39-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3be39-144">请求</span><span class="sxs-lookup"><span data-stu-id="3be39-144">Request</span></span>

<span data-ttu-id="3be39-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3be39-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="3be39-146">响应</span><span class="sxs-lookup"><span data-stu-id="3be39-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="3be39-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3be39-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "Azure Active Directory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
