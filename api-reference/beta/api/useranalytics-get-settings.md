---
title: 获取用户分析的设置
description: 检索 user analytics 的 settings 对象的属性。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: eb88e2ca480a448bee5fe0c6ebc9f2cba0ee9d0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022070"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="c8c4c-103">获取用户分析的设置</span><span class="sxs-lookup"><span data-stu-id="c8c4c-103">Get settings for user analytics</span></span>

<span data-ttu-id="c8c4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8c4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c4c-105">检索 [settings](../resources/settings.md) 对象的属性，使其适用于分析 API。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8c4c-106">权限</span><span class="sxs-lookup"><span data-stu-id="c8c4c-106">Permissions</span></span>

<span data-ttu-id="c8c4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8c4c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8c4c-109">Permission type</span></span>                        | <span data-ttu-id="c8c4c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8c4c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8c4c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c4c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8c4c-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c8c4c-112">User.Read</span></span> |
| <span data-ttu-id="c8c4c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c4c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c4c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-114">Not supported.</span></span> |
| <span data-ttu-id="c8c4c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8c4c-115">Application</span></span>                            | <span data-ttu-id="c8c4c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c4c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8c4c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8c4c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c8c4c-118">Optional query parameters</span></span>

<span data-ttu-id="c8c4c-119">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8c4c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8c4c-120">Request headers</span></span>

| <span data-ttu-id="c8c4c-121">名称</span><span class="sxs-lookup"><span data-stu-id="c8c4c-121">Name</span></span>      |<span data-ttu-id="c8c4c-122">说明</span><span class="sxs-lookup"><span data-stu-id="c8c4c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8c4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c4c-123">Authorization</span></span> | <span data-ttu-id="c8c4c-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c8c4c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8c4c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8c4c-125">Request body</span></span>

<span data-ttu-id="c8c4c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c4c-127">响应</span><span class="sxs-lookup"><span data-stu-id="c8c4c-127">Response</span></span>

<span data-ttu-id="c8c4c-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [设置](../resources/settings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8c4c-129">示例</span><span class="sxs-lookup"><span data-stu-id="c8c4c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8c4c-130">请求</span><span class="sxs-lookup"><span data-stu-id="c8c4c-130">Request</span></span>

<span data-ttu-id="c8c4c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8c4c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8c4c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="c8c4c-133">C#</span><span class="sxs-lookup"><span data-stu-id="c8c4c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8c4c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8c4c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8c4c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8c4c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8c4c-136">响应</span><span class="sxs-lookup"><span data-stu-id="c8c4c-136">Response</span></span>

<span data-ttu-id="c8c4c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c8c4c-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.settings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('12ab2b12-4b1a-43a1-adac-1a123456cd78')/analytics/settings",
    "hasLicense": true,
    "hasOptedOut": false,
    "hasGraphMailbox": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


