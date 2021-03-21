---
title: 获取用户分析的设置
description: 检索设置对象的属性以用于用户分析。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 607ddeea17942211cbd9988f5f3248385a0c7283
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955301"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="c45d6-103">获取用户分析的设置</span><span class="sxs-lookup"><span data-stu-id="c45d6-103">Get settings for user analytics</span></span>

<span data-ttu-id="c45d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c45d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c45d6-105">检索 [适用于分析](../resources/settings.md) API 的设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c45d6-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c45d6-106">权限</span><span class="sxs-lookup"><span data-stu-id="c45d6-106">Permissions</span></span>

<span data-ttu-id="c45d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c45d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c45d6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c45d6-109">Permission type</span></span>                        | <span data-ttu-id="c45d6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c45d6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c45d6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c45d6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c45d6-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c45d6-112">User.Read</span></span> |
| <span data-ttu-id="c45d6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c45d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c45d6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c45d6-114">Not supported.</span></span> |
| <span data-ttu-id="c45d6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c45d6-115">Application</span></span>                            | <span data-ttu-id="c45d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c45d6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c45d6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c45d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c45d6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c45d6-118">Optional query parameters</span></span>

<span data-ttu-id="c45d6-119">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="c45d6-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c45d6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c45d6-120">Request headers</span></span>

| <span data-ttu-id="c45d6-121">名称</span><span class="sxs-lookup"><span data-stu-id="c45d6-121">Name</span></span>      |<span data-ttu-id="c45d6-122">说明</span><span class="sxs-lookup"><span data-stu-id="c45d6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c45d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c45d6-123">Authorization</span></span> | <span data-ttu-id="c45d6-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c45d6-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c45d6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c45d6-125">Request body</span></span>

<span data-ttu-id="c45d6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c45d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c45d6-127">响应</span><span class="sxs-lookup"><span data-stu-id="c45d6-127">Response</span></span>

<span data-ttu-id="c45d6-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/settings.md)请求的设置对象。</span><span class="sxs-lookup"><span data-stu-id="c45d6-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c45d6-129">示例</span><span class="sxs-lookup"><span data-stu-id="c45d6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c45d6-130">请求</span><span class="sxs-lookup"><span data-stu-id="c45d6-130">Request</span></span>

<span data-ttu-id="c45d6-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c45d6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c45d6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c45d6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="c45d6-133">C#</span><span class="sxs-lookup"><span data-stu-id="c45d6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c45d6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c45d6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c45d6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c45d6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c45d6-136">Java</span><span class="sxs-lookup"><span data-stu-id="c45d6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c45d6-137">响应</span><span class="sxs-lookup"><span data-stu-id="c45d6-137">Response</span></span>

<span data-ttu-id="c45d6-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c45d6-138">The following is an example of the response.</span></span>

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


