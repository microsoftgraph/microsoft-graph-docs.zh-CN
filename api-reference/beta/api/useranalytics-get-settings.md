---
title: 获取用户分析的设置
description: 检索 user analytics 的 settings 对象的属性。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d44203c1d0a2a910182822cfc35565a30e1cd4ae
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724104"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="1a1b8-103">获取用户分析的设置</span><span class="sxs-lookup"><span data-stu-id="1a1b8-103">Get settings for user analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a1b8-104">检索[settings](../resources/settings.md)对象的属性, 使其适用于分析 API。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-104">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a1b8-105">权限</span><span class="sxs-lookup"><span data-stu-id="1a1b8-105">Permissions</span></span>

<span data-ttu-id="1a1b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a1b8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a1b8-108">Permission type</span></span>                        | <span data-ttu-id="1a1b8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a1b8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a1b8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a1b8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a1b8-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="1a1b8-111">User.Read</span></span> |
| <span data-ttu-id="1a1b8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a1b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a1b8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-113">Not supported.</span></span> |
| <span data-ttu-id="1a1b8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a1b8-114">Application</span></span>                            | <span data-ttu-id="1a1b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a1b8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a1b8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET https://graph.microsoft.com/beta/me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a1b8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a1b8-117">Optional query parameters</span></span>

<span data-ttu-id="1a1b8-118">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a1b8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a1b8-119">Request headers</span></span>

| <span data-ttu-id="1a1b8-120">名称</span><span class="sxs-lookup"><span data-stu-id="1a1b8-120">Name</span></span>      |<span data-ttu-id="1a1b8-121">说明</span><span class="sxs-lookup"><span data-stu-id="1a1b8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a1b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a1b8-122">Authorization</span></span> | <span data-ttu-id="1a1b8-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1a1b8-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a1b8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a1b8-124">Request body</span></span>

<span data-ttu-id="1a1b8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a1b8-126">响应</span><span class="sxs-lookup"><span data-stu-id="1a1b8-126">Response</span></span>

<span data-ttu-id="1a1b8-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[设置](../resources/settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-127">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a1b8-128">示例</span><span class="sxs-lookup"><span data-stu-id="1a1b8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a1b8-129">请求</span><span class="sxs-lookup"><span data-stu-id="1a1b8-129">Request</span></span>

<span data-ttu-id="1a1b8-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a1b8-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1a1b8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a1b8-132">C#</span><span class="sxs-lookup"><span data-stu-id="1a1b8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a1b8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a1b8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a1b8-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="1a1b8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a1b8-135">响应</span><span class="sxs-lookup"><span data-stu-id="1a1b8-135">Response</span></span>

<span data-ttu-id="1a1b8-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a1b8-136">The following is an example of the response.</span></span>

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
