---
title: 列出 applicationTemplates
description: 检索 applicationtemplate 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2baa42a7bc985aec6deae580cfd5a4db59e0818d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441366"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="c7f18-103">列出 applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="c7f18-103">List applicationTemplates</span></span>

<span data-ttu-id="c7f18-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c7f18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7f18-105">从 Azure AD 应用程序库中检索[applicationTemplate](../resources/applicationtemplate.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c7f18-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7f18-106">权限</span><span class="sxs-lookup"><span data-stu-id="c7f18-106">Permissions</span></span>

<span data-ttu-id="c7f18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7f18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7f18-109">Permission type</span></span>                        | <span data-ttu-id="c7f18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7f18-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7f18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7f18-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7f18-112">无。</span><span class="sxs-lookup"><span data-stu-id="c7f18-112">None.</span></span> |
| <span data-ttu-id="c7f18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7f18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7f18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7f18-114">Not supported.</span></span> |
| <span data-ttu-id="c7f18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7f18-115">Application</span></span>                            | <span data-ttu-id="c7f18-116">无。</span><span class="sxs-lookup"><span data-stu-id="c7f18-116">None.</span></span> |

<span data-ttu-id="c7f18-117">只要您的应用程序具有有效的访问令牌以调用 Microsoft Graph，就不需要额外的权限即可调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c7f18-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7f18-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7f18-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7f18-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7f18-119">Optional query parameters</span></span>

<span data-ttu-id="c7f18-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7f18-120">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="c7f18-121">您可以在有限`$filter`的方式中使用该参数。</span><span class="sxs-lookup"><span data-stu-id="c7f18-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="c7f18-122">只能按**displayName**或**类别**进行筛选。</span><span class="sxs-lookup"><span data-stu-id="c7f18-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="c7f18-123">例如， `$filter=contains(displayName, 'salesf')` 或 `$filter=categories/any(c:contains(c, 'myCategory'))`。</span><span class="sxs-lookup"><span data-stu-id="c7f18-123">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="c7f18-124">可以在任何`$orderby`GET `$top,`请求`$skip`中使用和查询参数。</span><span class="sxs-lookup"><span data-stu-id="c7f18-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="c7f18-125">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c7f18-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7f18-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7f18-126">Request headers</span></span>

| <span data-ttu-id="c7f18-127">名称</span><span class="sxs-lookup"><span data-stu-id="c7f18-127">Name</span></span>      |<span data-ttu-id="c7f18-128">说明</span><span class="sxs-lookup"><span data-stu-id="c7f18-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7f18-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7f18-129">Authorization</span></span> | <span data-ttu-id="c7f18-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c7f18-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7f18-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7f18-131">Request body</span></span>

<span data-ttu-id="c7f18-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7f18-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7f18-133">响应</span><span class="sxs-lookup"><span data-stu-id="c7f18-133">Response</span></span>

<span data-ttu-id="c7f18-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和[applicationTemplate](../resources/applicationtemplate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c7f18-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7f18-135">示例</span><span class="sxs-lookup"><span data-stu-id="c7f18-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7f18-136">请求</span><span class="sxs-lookup"><span data-stu-id="c7f18-136">Request</span></span>

<span data-ttu-id="c7f18-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7f18-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7f18-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7f18-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="c7f18-139">C#</span><span class="sxs-lookup"><span data-stu-id="c7f18-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7f18-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7f18-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7f18-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7f18-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7f18-142">响应</span><span class="sxs-lookup"><span data-stu-id="c7f18-142">Response</span></span>

<span data-ttu-id="c7f18-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c7f18-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c7f18-144">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c7f18-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c7f18-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7f18-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applicationTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
