---
title: 列出 applicationTemplates
description: 检索 applicationtemplate 对象的列表。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac8ad3a8b4a7a396c0cb35c1c72c2d1a2e309184
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147893"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="02406-103">列出 applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="02406-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02406-104">从 Azure AD 应用程序库中检索[applicationTemplate](../resources/applicationtemplate.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="02406-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="02406-105">权限</span><span class="sxs-lookup"><span data-stu-id="02406-105">Permissions</span></span>

<span data-ttu-id="02406-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02406-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="02406-108">Permission type</span></span>                        | <span data-ttu-id="02406-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02406-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02406-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02406-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02406-111">无。</span><span class="sxs-lookup"><span data-stu-id="02406-111">None.</span></span> |
| <span data-ttu-id="02406-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02406-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02406-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="02406-113">Not supported.</span></span> |
| <span data-ttu-id="02406-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="02406-114">Application</span></span>                            | <span data-ttu-id="02406-115">无。</span><span class="sxs-lookup"><span data-stu-id="02406-115">None.</span></span> |

<span data-ttu-id="02406-116">只要您的应用程序具有有效的访问令牌以调用 Microsoft Graph, 就不需要额外的权限即可调用此 API。</span><span class="sxs-lookup"><span data-stu-id="02406-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="02406-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02406-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02406-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="02406-118">Optional query parameters</span></span>

<span data-ttu-id="02406-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="02406-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="02406-120">您可以在有限`$filter`的方式中使用该参数。</span><span class="sxs-lookup"><span data-stu-id="02406-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="02406-121">只能按**displayName**或**类别**进行筛选。</span><span class="sxs-lookup"><span data-stu-id="02406-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="02406-122">例如， `$filter=contains(displayName, 'salesf')` 或 `$filter=categories/any(c:contains(c, 'myCategory'))`。</span><span class="sxs-lookup"><span data-stu-id="02406-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="02406-123">可以在任何`$orderby`GET `$top,`请求`$skip`中使用和查询参数。</span><span class="sxs-lookup"><span data-stu-id="02406-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="02406-124">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="02406-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="02406-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="02406-125">Request headers</span></span>

| <span data-ttu-id="02406-126">名称</span><span class="sxs-lookup"><span data-stu-id="02406-126">Name</span></span>      |<span data-ttu-id="02406-127">说明</span><span class="sxs-lookup"><span data-stu-id="02406-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02406-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="02406-128">Authorization</span></span> | <span data-ttu-id="02406-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="02406-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="02406-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="02406-130">Request body</span></span>

<span data-ttu-id="02406-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02406-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02406-132">响应</span><span class="sxs-lookup"><span data-stu-id="02406-132">Response</span></span>

<span data-ttu-id="02406-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[applicationTemplate](../resources/applicationtemplate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="02406-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02406-134">示例</span><span class="sxs-lookup"><span data-stu-id="02406-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02406-135">请求</span><span class="sxs-lookup"><span data-stu-id="02406-135">Request</span></span>

<span data-ttu-id="02406-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02406-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```

### <a name="response"></a><span data-ttu-id="02406-137">响应</span><span class="sxs-lookup"><span data-stu-id="02406-137">Response</span></span>

<span data-ttu-id="02406-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="02406-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="02406-139">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="02406-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="02406-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="02406-140">All the properties will be returned from an actual call.</span></span>

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
