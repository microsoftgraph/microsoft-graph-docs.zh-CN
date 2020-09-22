---
title: 获取 applicationTemplate
description: 检索 applicationtemplate 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 21c350a3ed5b1ca11257c7fc5e2fe53fed785920
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996670"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="10fdb-103">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="10fdb-103">Get applicationTemplate</span></span>

<span data-ttu-id="10fdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10fdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10fdb-105">检索 [applicationTemplate](../resources/applicationtemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10fdb-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10fdb-106">权限</span><span class="sxs-lookup"><span data-stu-id="10fdb-106">Permissions</span></span>

<span data-ttu-id="10fdb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10fdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10fdb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="10fdb-109">Permission type</span></span>                        | <span data-ttu-id="10fdb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10fdb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10fdb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10fdb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10fdb-112">无。</span><span class="sxs-lookup"><span data-stu-id="10fdb-112">None.</span></span> |
| <span data-ttu-id="10fdb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10fdb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10fdb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="10fdb-114">Not supported.</span></span> |
| <span data-ttu-id="10fdb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="10fdb-115">Application</span></span>                            | <span data-ttu-id="10fdb-116">无。</span><span class="sxs-lookup"><span data-stu-id="10fdb-116">None.</span></span> |

<span data-ttu-id="10fdb-117">只要您的应用程序具有有效的访问令牌以调用 Microsoft Graph，就不需要额外的权限即可调用此 API。</span><span class="sxs-lookup"><span data-stu-id="10fdb-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="10fdb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10fdb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10fdb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10fdb-119">Optional query parameters</span></span>

<span data-ttu-id="10fdb-120">您可以使用 `$select` 查询参数来仅指定所需的属性以获得最佳性能。</span><span class="sxs-lookup"><span data-stu-id="10fdb-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="10fdb-121">始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="10fdb-121">The **id** property is always returned.</span></span> 

<span data-ttu-id="10fdb-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="10fdb-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="10fdb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="10fdb-123">Request headers</span></span>

| <span data-ttu-id="10fdb-124">名称</span><span class="sxs-lookup"><span data-stu-id="10fdb-124">Name</span></span>      |<span data-ttu-id="10fdb-125">说明</span><span class="sxs-lookup"><span data-stu-id="10fdb-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10fdb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="10fdb-126">Authorization</span></span> | <span data-ttu-id="10fdb-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="10fdb-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10fdb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="10fdb-128">Request body</span></span>

<span data-ttu-id="10fdb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10fdb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10fdb-130">响应</span><span class="sxs-lookup"><span data-stu-id="10fdb-130">Response</span></span>

<span data-ttu-id="10fdb-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [applicationTemplate](../resources/applicationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10fdb-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10fdb-132">示例</span><span class="sxs-lookup"><span data-stu-id="10fdb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10fdb-133">请求</span><span class="sxs-lookup"><span data-stu-id="10fdb-133">Request</span></span>

<span data-ttu-id="10fdb-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="10fdb-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10fdb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="10fdb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="10fdb-136">C#</span><span class="sxs-lookup"><span data-stu-id="10fdb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10fdb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10fdb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10fdb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10fdb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10fdb-139">响应</span><span class="sxs-lookup"><span data-stu-id="10fdb-139">Response</span></span>

<span data-ttu-id="10fdb-140">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="10fdb-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="10fdb-141">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10fdb-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10fdb-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="10fdb-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


