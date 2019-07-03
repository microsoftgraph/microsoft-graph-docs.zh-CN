---
title: 列出 applicationTemplates
description: 检索 applicationtemplate 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d74e274d2db8d20cb9cf3269ab78cc12055b76c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439516"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="315d9-103">列出 applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="315d9-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="315d9-104">从 Azure AD 应用程序库中检索[applicationTemplate](../resources/applicationtemplate.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="315d9-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="315d9-105">权限</span><span class="sxs-lookup"><span data-stu-id="315d9-105">Permissions</span></span>

<span data-ttu-id="315d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="315d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="315d9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="315d9-108">Permission type</span></span>                        | <span data-ttu-id="315d9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="315d9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="315d9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="315d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="315d9-111">无。</span><span class="sxs-lookup"><span data-stu-id="315d9-111">None.</span></span> |
| <span data-ttu-id="315d9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="315d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="315d9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="315d9-113">Not supported.</span></span> |
| <span data-ttu-id="315d9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="315d9-114">Application</span></span>                            | <span data-ttu-id="315d9-115">无。</span><span class="sxs-lookup"><span data-stu-id="315d9-115">None.</span></span> |

<span data-ttu-id="315d9-116">只要您的应用程序具有有效的访问令牌以调用 Microsoft Graph, 就不需要额外的权限即可调用此 API。</span><span class="sxs-lookup"><span data-stu-id="315d9-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="315d9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="315d9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="315d9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="315d9-118">Optional query parameters</span></span>

<span data-ttu-id="315d9-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="315d9-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="315d9-120">您可以在有限`$filter`的方式中使用该参数。</span><span class="sxs-lookup"><span data-stu-id="315d9-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="315d9-121">只能按**displayName**或**类别**进行筛选。</span><span class="sxs-lookup"><span data-stu-id="315d9-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="315d9-122">例如， `$filter=contains(displayName, 'salesf')` 或 `$filter=categories/any(c:contains(c, 'myCategory'))`。</span><span class="sxs-lookup"><span data-stu-id="315d9-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="315d9-123">可以在任何`$orderby`GET `$top,`请求`$skip`中使用和查询参数。</span><span class="sxs-lookup"><span data-stu-id="315d9-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="315d9-124">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="315d9-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="315d9-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="315d9-125">Request headers</span></span>

| <span data-ttu-id="315d9-126">名称</span><span class="sxs-lookup"><span data-stu-id="315d9-126">Name</span></span>      |<span data-ttu-id="315d9-127">说明</span><span class="sxs-lookup"><span data-stu-id="315d9-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="315d9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="315d9-128">Authorization</span></span> | <span data-ttu-id="315d9-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="315d9-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="315d9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="315d9-130">Request body</span></span>

<span data-ttu-id="315d9-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="315d9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="315d9-132">响应</span><span class="sxs-lookup"><span data-stu-id="315d9-132">Response</span></span>

<span data-ttu-id="315d9-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[applicationTemplate](../resources/applicationtemplate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="315d9-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="315d9-134">示例</span><span class="sxs-lookup"><span data-stu-id="315d9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="315d9-135">请求</span><span class="sxs-lookup"><span data-stu-id="315d9-135">Request</span></span>

<span data-ttu-id="315d9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="315d9-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="315d9-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="315d9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="315d9-138">C#</span><span class="sxs-lookup"><span data-stu-id="315d9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="315d9-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="315d9-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="315d9-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="315d9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="315d9-141">响应</span><span class="sxs-lookup"><span data-stu-id="315d9-141">Response</span></span>

<span data-ttu-id="315d9-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="315d9-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="315d9-143">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="315d9-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="315d9-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="315d9-144">All the properties will be returned from an actual call.</span></span>

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
