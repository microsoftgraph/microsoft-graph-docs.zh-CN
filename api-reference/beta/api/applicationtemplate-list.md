---
title: 列出 applicationTemplates
description: 检索 applicationtemplate 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ebd1b178ad1a6ea0e178ab582439ace433951ffb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471532"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="2afc2-103">列出 applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="2afc2-103">List applicationTemplates</span></span>

<span data-ttu-id="2afc2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2afc2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2afc2-105">从 Azure AD 应用程序库检索 [applicationTemplate](../resources/applicationtemplate.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2afc2-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="2afc2-106">权限</span><span class="sxs-lookup"><span data-stu-id="2afc2-106">Permissions</span></span>

<span data-ttu-id="2afc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2afc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2afc2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2afc2-109">Permission type</span></span>                        | <span data-ttu-id="2afc2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2afc2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2afc2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2afc2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2afc2-112">无。</span><span class="sxs-lookup"><span data-stu-id="2afc2-112">None.</span></span> |
| <span data-ttu-id="2afc2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2afc2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2afc2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2afc2-114">Not supported.</span></span> |
| <span data-ttu-id="2afc2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2afc2-115">Application</span></span>                            | <span data-ttu-id="2afc2-116">无。</span><span class="sxs-lookup"><span data-stu-id="2afc2-116">None.</span></span> |

<span data-ttu-id="2afc2-117">调用此 API 不需要其他权限，只要您的应用程序具有调用 Microsoft Graph 的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2afc2-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="2afc2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2afc2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2afc2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2afc2-119">Optional query parameters</span></span>

<span data-ttu-id="2afc2-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2afc2-120">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="2afc2-121">可以有限 `$filter` 的方式使用参数。</span><span class="sxs-lookup"><span data-stu-id="2afc2-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="2afc2-122">只能按 **displayName** 或类别 **进行筛选**。</span><span class="sxs-lookup"><span data-stu-id="2afc2-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="2afc2-123">例如， `$filter=contains(displayName, 'salesf')` 或 `$filter=categories/any(c:contains(c, 'myCategory'))`。</span><span class="sxs-lookup"><span data-stu-id="2afc2-123">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="2afc2-124">可以在任何 `$orderby` `$top,` GET 请求中 `$skip` 使用和查询参数。</span><span class="sxs-lookup"><span data-stu-id="2afc2-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="2afc2-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2afc2-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2afc2-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2afc2-126">Request headers</span></span>

| <span data-ttu-id="2afc2-127">名称</span><span class="sxs-lookup"><span data-stu-id="2afc2-127">Name</span></span>      |<span data-ttu-id="2afc2-128">说明</span><span class="sxs-lookup"><span data-stu-id="2afc2-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2afc2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2afc2-129">Authorization</span></span> | <span data-ttu-id="2afc2-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2afc2-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2afc2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="2afc2-131">Request body</span></span>

<span data-ttu-id="2afc2-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2afc2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2afc2-133">响应</span><span class="sxs-lookup"><span data-stu-id="2afc2-133">Response</span></span>

<span data-ttu-id="2afc2-134">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [applicationTemplate](../resources/applicationtemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2afc2-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2afc2-135">示例</span><span class="sxs-lookup"><span data-stu-id="2afc2-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2afc2-136">请求</span><span class="sxs-lookup"><span data-stu-id="2afc2-136">Request</span></span>

<span data-ttu-id="2afc2-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2afc2-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2afc2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2afc2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="2afc2-139">C#</span><span class="sxs-lookup"><span data-stu-id="2afc2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2afc2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2afc2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2afc2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2afc2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2afc2-142">Java</span><span class="sxs-lookup"><span data-stu-id="2afc2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2afc2-143">响应</span><span class="sxs-lookup"><span data-stu-id="2afc2-143">Response</span></span>

<span data-ttu-id="2afc2-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2afc2-144">The following is an example of the response.</span></span>

> <span data-ttu-id="2afc2-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2afc2-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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



