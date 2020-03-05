---
title: 获取 applicationTemplate
description: 检索 applicationtemplate 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbf38412fc6442ffcc0a7037e2a1dcde30a35469
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441401"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="d0cee-103">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="d0cee-103">Get applicationTemplate</span></span>

<span data-ttu-id="d0cee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d0cee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0cee-105">检索[applicationTemplate](../resources/applicationtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d0cee-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0cee-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0cee-106">Permissions</span></span>

<span data-ttu-id="d0cee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0cee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0cee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0cee-109">Permission type</span></span>                        | <span data-ttu-id="d0cee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0cee-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0cee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0cee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0cee-112">无。</span><span class="sxs-lookup"><span data-stu-id="d0cee-112">None.</span></span> |
| <span data-ttu-id="d0cee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0cee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0cee-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0cee-114">Not supported.</span></span> |
| <span data-ttu-id="d0cee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0cee-115">Application</span></span>                            | <span data-ttu-id="d0cee-116">无。</span><span class="sxs-lookup"><span data-stu-id="d0cee-116">None.</span></span> |

<span data-ttu-id="d0cee-117">只要您的应用程序具有有效的访问令牌以调用 Microsoft Graph，就不需要额外的权限即可调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d0cee-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0cee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0cee-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0cee-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d0cee-119">Optional query parameters</span></span>

<span data-ttu-id="d0cee-120">您可以使用`$select`查询参数来仅指定所需的属性以获得最佳性能。</span><span class="sxs-lookup"><span data-stu-id="d0cee-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="d0cee-121">始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="d0cee-121">The **id** property is always returned.</span></span> 

<span data-ttu-id="d0cee-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d0cee-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0cee-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0cee-123">Request headers</span></span>

| <span data-ttu-id="d0cee-124">名称</span><span class="sxs-lookup"><span data-stu-id="d0cee-124">Name</span></span>      |<span data-ttu-id="d0cee-125">说明</span><span class="sxs-lookup"><span data-stu-id="d0cee-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0cee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0cee-126">Authorization</span></span> | <span data-ttu-id="d0cee-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d0cee-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0cee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0cee-128">Request body</span></span>

<span data-ttu-id="d0cee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0cee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0cee-130">响应</span><span class="sxs-lookup"><span data-stu-id="d0cee-130">Response</span></span>

<span data-ttu-id="d0cee-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[applicationTemplate](../resources/applicationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0cee-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0cee-132">示例</span><span class="sxs-lookup"><span data-stu-id="d0cee-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0cee-133">请求</span><span class="sxs-lookup"><span data-stu-id="d0cee-133">Request</span></span>

<span data-ttu-id="d0cee-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d0cee-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0cee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0cee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="d0cee-136">C#</span><span class="sxs-lookup"><span data-stu-id="d0cee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0cee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0cee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0cee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0cee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0cee-139">响应</span><span class="sxs-lookup"><span data-stu-id="d0cee-139">Response</span></span>

<span data-ttu-id="d0cee-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d0cee-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d0cee-141">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0cee-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0cee-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d0cee-142">All the properties will be returned from an actual call.</span></span>

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
