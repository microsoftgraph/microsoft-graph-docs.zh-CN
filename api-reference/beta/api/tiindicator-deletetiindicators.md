---
title: 'tiIndicator: deleteTiIndicators'
description: 在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 98059d636e58ad0fc4f9bccc2587b50a72e5b3d3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637575"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="4331d-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="4331d-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4331d-104">在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="4331d-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="4331d-105">权限</span><span class="sxs-lookup"><span data-stu-id="4331d-105">Permissions</span></span>

<span data-ttu-id="4331d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4331d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4331d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4331d-108">Permission type</span></span> | <span data-ttu-id="4331d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4331d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4331d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4331d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4331d-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4331d-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="4331d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4331d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4331d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4331d-113">Not supported.</span></span> |
| <span data-ttu-id="4331d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4331d-114">Application</span></span>                            | <span data-ttu-id="4331d-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4331d-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="4331d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4331d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="4331d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4331d-117">Request headers</span></span>

| <span data-ttu-id="4331d-118">名称</span><span class="sxs-lookup"><span data-stu-id="4331d-118">Name</span></span>          | <span data-ttu-id="4331d-119">说明</span><span class="sxs-lookup"><span data-stu-id="4331d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4331d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4331d-120">Authorization</span></span> | <span data-ttu-id="4331d-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4331d-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4331d-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="4331d-122">Request body</span></span>

<span data-ttu-id="4331d-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4331d-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4331d-124">参数</span><span class="sxs-lookup"><span data-stu-id="4331d-124">Parameter</span></span>    | <span data-ttu-id="4331d-125">类型</span><span class="sxs-lookup"><span data-stu-id="4331d-125">Type</span></span>        | <span data-ttu-id="4331d-126">说明</span><span class="sxs-lookup"><span data-stu-id="4331d-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4331d-127">值</span><span class="sxs-lookup"><span data-stu-id="4331d-127">value</span></span>|<span data-ttu-id="4331d-128">String collection</span><span class="sxs-lookup"><span data-stu-id="4331d-128">String collection</span></span>| <span data-ttu-id="4331d-129">要删除的`id`TiIndicator 的集合。</span><span class="sxs-lookup"><span data-stu-id="4331d-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="4331d-130">响应</span><span class="sxs-lookup"><span data-stu-id="4331d-130">Response</span></span>

<span data-ttu-id="4331d-131">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[resultInfo](../resources/resultinfo.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="4331d-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4331d-132">示例</span><span class="sxs-lookup"><span data-stu-id="4331d-132">Examples</span></span>

<span data-ttu-id="4331d-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4331d-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4331d-134">请求</span><span class="sxs-lookup"><span data-stu-id="4331d-134">Request</span></span>

<span data-ttu-id="4331d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4331d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4331d-136">响应</span><span class="sxs-lookup"><span data-stu-id="4331d-136">Response</span></span>

<span data-ttu-id="4331d-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4331d-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4331d-138">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4331d-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4331d-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4331d-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4331d-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4331d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4331d-141">语言</span><span class="sxs-lookup"><span data-stu-id="4331d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4331d-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="4331d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
