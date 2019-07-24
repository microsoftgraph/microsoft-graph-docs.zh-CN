---
title: 获取 publishedResource
description: 检索[publishedResource](../resources/publishedresource.md)对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b59b43cb54f70291fc939ff58b7f88d191c89420
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841001"
---
# <a name="get-publishedresource"></a><span data-ttu-id="5456c-103">获取 publishedResource</span><span class="sxs-lookup"><span data-stu-id="5456c-103">Get publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5456c-104">检索[publishedResource](../resources/publishedresource.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5456c-104">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5456c-105">权限</span><span class="sxs-lookup"><span data-stu-id="5456c-105">Permissions</span></span>

<span data-ttu-id="5456c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5456c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5456c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5456c-108">Permission type</span></span>                        | <span data-ttu-id="5456c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5456c-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="5456c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5456c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5456c-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="5456c-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5456c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5456c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5456c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5456c-113">Not supported.</span></span> |
| <span data-ttu-id="5456c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5456c-114">Application</span></span>                            | <span data-ttu-id="5456c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5456c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5456c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5456c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5456c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5456c-117">Optional query parameters</span></span>

<span data-ttu-id="5456c-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5456c-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5456c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5456c-119">Request headers</span></span>

| <span data-ttu-id="5456c-120">名称</span><span class="sxs-lookup"><span data-stu-id="5456c-120">Name</span></span>      |<span data-ttu-id="5456c-121">说明</span><span class="sxs-lookup"><span data-stu-id="5456c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5456c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5456c-122">Authorization</span></span> | <span data-ttu-id="5456c-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5456c-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5456c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5456c-124">Request body</span></span>

<span data-ttu-id="5456c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5456c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5456c-126">响应</span><span class="sxs-lookup"><span data-stu-id="5456c-126">Response</span></span>

<span data-ttu-id="5456c-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5456c-127">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5456c-128">示例</span><span class="sxs-lookup"><span data-stu-id="5456c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5456c-129">请求</span><span class="sxs-lookup"><span data-stu-id="5456c-129">Request</span></span>

<span data-ttu-id="5456c-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5456c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```

### <a name="response"></a><span data-ttu-id="5456c-131">响应</span><span class="sxs-lookup"><span data-stu-id="5456c-131">Response</span></span>

<span data-ttu-id="5456c-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5456c-132">The following is an example of the response.</span></span>

> <span data-ttu-id="5456c-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5456c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "publishingType": "provisioning",
    "displayName": "Demo provisioning",
    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
    "resourceName": "domain1.contoso.com",
    "agentGroups": [
        {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
