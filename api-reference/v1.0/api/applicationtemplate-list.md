---
title: 列出 applicationTemplates
description: 检索 applicationtemplate 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7d8a80b6f2cee8726f50cf32a7c5c6efa5e947c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775139"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="e4455-103">列出 applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="e4455-103">List applicationTemplates</span></span>

<span data-ttu-id="e4455-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4455-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4455-105">从 Azure AD 应用程序库中检索 [applicationTemplate](../resources/applicationtemplate.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e4455-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4455-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4455-106">Permissions</span></span>

<span data-ttu-id="e4455-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4455-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4455-109">Permission type</span></span>                        | <span data-ttu-id="e4455-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4455-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e4455-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4455-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4455-112">无。</span><span class="sxs-lookup"><span data-stu-id="e4455-112">None.</span></span>                                       |
| <span data-ttu-id="e4455-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4455-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4455-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4455-114">Not supported.</span></span>                              |
| <span data-ttu-id="e4455-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4455-115">Application</span></span>                            | <span data-ttu-id="e4455-116">无。</span><span class="sxs-lookup"><span data-stu-id="e4455-116">None.</span></span>                                       |

<span data-ttu-id="e4455-117">调用此 API 不需要其他权限，只要应用程序具有有效的访问令牌来调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="e4455-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="e4455-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4455-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4455-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e4455-119">Optional query parameters</span></span>

<span data-ttu-id="e4455-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e4455-120">This method supports some of the OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="e4455-121">可以有限 `$filter` 的方式使用 参数。</span><span class="sxs-lookup"><span data-stu-id="e4455-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="e4455-122">只能按 **displayName 或 categories** **进行筛选**。</span><span class="sxs-lookup"><span data-stu-id="e4455-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="e4455-123">例如， `$filter=contains(displayName, 'salesf')` `$filter=categories/any(c:contains(c, 'myCategory'))` 或 。</span><span class="sxs-lookup"><span data-stu-id="e4455-123">For example, `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="e4455-124">可以在任何 `$orderby` `$top,` GET 请求 `$skip` 中使用 和 查询参数。</span><span class="sxs-lookup"><span data-stu-id="e4455-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="e4455-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e4455-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4455-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4455-126">Request headers</span></span>

| <span data-ttu-id="e4455-127">名称</span><span class="sxs-lookup"><span data-stu-id="e4455-127">Name</span></span>          | <span data-ttu-id="e4455-128">说明</span><span class="sxs-lookup"><span data-stu-id="e4455-128">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="e4455-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4455-129">Authorization</span></span> | <span data-ttu-id="e4455-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e4455-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4455-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4455-131">Request body</span></span>

<span data-ttu-id="e4455-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4455-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4455-133">响应</span><span class="sxs-lookup"><span data-stu-id="e4455-133">Response</span></span>

<span data-ttu-id="e4455-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [applicationTemplate](../resources/applicationtemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e4455-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4455-135">示例</span><span class="sxs-lookup"><span data-stu-id="e4455-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4455-136">请求</span><span class="sxs-lookup"><span data-stu-id="e4455-136">Request</span></span>

<span data-ttu-id="e4455-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e4455-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4455-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4455-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="e4455-139">C#</span><span class="sxs-lookup"><span data-stu-id="e4455-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4455-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4455-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4455-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4455-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4455-142">Java</span><span class="sxs-lookup"><span data-stu-id="e4455-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4455-143">响应</span><span class="sxs-lookup"><span data-stu-id="e4455-143">Response</span></span>

<span data-ttu-id="e4455-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e4455-144">The following is an example of the response.</span></span>

> <span data-ttu-id="e4455-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4455-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
