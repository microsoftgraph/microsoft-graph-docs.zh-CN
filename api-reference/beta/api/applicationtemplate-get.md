---
title: 获取 applicationTemplate
description: 检索 applicationtemplate 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e32439d98961a95ef98113f86833eec2c38dc869
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318640"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="48695-103">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="48695-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48695-104">检索[applicationTemplate](../resources/applicationtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48695-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48695-105">权限</span><span class="sxs-lookup"><span data-stu-id="48695-105">Permissions</span></span>

<span data-ttu-id="48695-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48695-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="48695-108">Permission type</span></span>                        | <span data-ttu-id="48695-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48695-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48695-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48695-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="48695-111">无。</span><span class="sxs-lookup"><span data-stu-id="48695-111">None.</span></span> |
| <span data-ttu-id="48695-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48695-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48695-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="48695-113">Not supported.</span></span> |
| <span data-ttu-id="48695-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="48695-114">Application</span></span>                            | <span data-ttu-id="48695-115">无。</span><span class="sxs-lookup"><span data-stu-id="48695-115">None.</span></span> |

<span data-ttu-id="48695-116">只要您的应用程序具有有效的访问令牌以调用 Microsoft Graph, 就不需要额外的权限即可调用此 API。</span><span class="sxs-lookup"><span data-stu-id="48695-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="48695-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48695-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48695-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="48695-118">Optional query parameters</span></span>

<span data-ttu-id="48695-119">您可以使用`$select`查询参数来仅指定所需的属性以获得最佳性能。</span><span class="sxs-lookup"><span data-stu-id="48695-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="48695-120">始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="48695-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="48695-121">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="48695-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="48695-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="48695-122">Request headers</span></span>

| <span data-ttu-id="48695-123">名称</span><span class="sxs-lookup"><span data-stu-id="48695-123">Name</span></span>      |<span data-ttu-id="48695-124">说明</span><span class="sxs-lookup"><span data-stu-id="48695-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48695-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="48695-125">Authorization</span></span> | <span data-ttu-id="48695-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="48695-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="48695-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="48695-127">Request body</span></span>

<span data-ttu-id="48695-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48695-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48695-129">响应</span><span class="sxs-lookup"><span data-stu-id="48695-129">Response</span></span>

<span data-ttu-id="48695-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[applicationTemplate](../resources/applicationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48695-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48695-131">示例</span><span class="sxs-lookup"><span data-stu-id="48695-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48695-132">请求</span><span class="sxs-lookup"><span data-stu-id="48695-132">Request</span></span>

<span data-ttu-id="48695-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48695-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48695-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="48695-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48695-135">C#</span><span class="sxs-lookup"><span data-stu-id="48695-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48695-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48695-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48695-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="48695-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="48695-138">Java</span><span class="sxs-lookup"><span data-stu-id="48695-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48695-139">响应</span><span class="sxs-lookup"><span data-stu-id="48695-139">Response</span></span>

<span data-ttu-id="48695-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="48695-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="48695-141">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="48695-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48695-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="48695-142">All the properties will be returned from an actual call.</span></span>

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
