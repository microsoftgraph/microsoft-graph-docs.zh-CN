---
title: 获取 applicationTemplate
description: 检索 applicationtemplate 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: db1957652d2abd29d79bce8c594b83deaf2992f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768879"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="859b2-103">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="859b2-103">Get applicationTemplate</span></span>

<span data-ttu-id="859b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="859b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="859b2-105">检索 [applicationTemplate 对象](../resources/applicationtemplate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="859b2-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="859b2-106">权限</span><span class="sxs-lookup"><span data-stu-id="859b2-106">Permissions</span></span>

<span data-ttu-id="859b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="859b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="859b2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="859b2-109">Permission type</span></span>                        | <span data-ttu-id="859b2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="859b2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="859b2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="859b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="859b2-112">无。</span><span class="sxs-lookup"><span data-stu-id="859b2-112">None.</span></span>                                       |
| <span data-ttu-id="859b2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="859b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="859b2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="859b2-114">Not supported.</span></span>                              |
| <span data-ttu-id="859b2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="859b2-115">Application</span></span>                            | <span data-ttu-id="859b2-116">无。</span><span class="sxs-lookup"><span data-stu-id="859b2-116">None.</span></span>                                       |

<span data-ttu-id="859b2-117">调用此 API 不需要其他权限，只要应用程序具有有效的访问令牌来调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="859b2-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="859b2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="859b2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="859b2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="859b2-119">Optional query parameters</span></span>

<span data-ttu-id="859b2-120">查询参数 `$select` 可用于仅指定获得最佳性能所需的属性。</span><span class="sxs-lookup"><span data-stu-id="859b2-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="859b2-121">始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="859b2-121">The **id** property is always returned.</span></span>

<span data-ttu-id="859b2-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="859b2-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="859b2-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="859b2-123">Request headers</span></span>

| <span data-ttu-id="859b2-124">名称</span><span class="sxs-lookup"><span data-stu-id="859b2-124">Name</span></span>          | <span data-ttu-id="859b2-125">说明</span><span class="sxs-lookup"><span data-stu-id="859b2-125">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="859b2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="859b2-126">Authorization</span></span> | <span data-ttu-id="859b2-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="859b2-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="859b2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="859b2-128">Request body</span></span>

<span data-ttu-id="859b2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="859b2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="859b2-130">响应</span><span class="sxs-lookup"><span data-stu-id="859b2-130">Response</span></span>

<span data-ttu-id="859b2-131">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [applicationTemplate](../resources/applicationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="859b2-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="859b2-132">示例</span><span class="sxs-lookup"><span data-stu-id="859b2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="859b2-133">请求</span><span class="sxs-lookup"><span data-stu-id="859b2-133">Request</span></span>

<span data-ttu-id="859b2-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="859b2-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="859b2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="859b2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="859b2-136">C#</span><span class="sxs-lookup"><span data-stu-id="859b2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="859b2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="859b2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="859b2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="859b2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="859b2-139">Java</span><span class="sxs-lookup"><span data-stu-id="859b2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="859b2-140">响应</span><span class="sxs-lookup"><span data-stu-id="859b2-140">Response</span></span>

<span data-ttu-id="859b2-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="859b2-141">The following is an example of the response.</span></span>

> <span data-ttu-id="859b2-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="859b2-142">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
