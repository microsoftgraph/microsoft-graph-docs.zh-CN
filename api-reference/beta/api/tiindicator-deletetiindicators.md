---
title: tiIndicator：deleteTiIndicators
description: 在一个 (而不是) 个请求中删除多个威胁情报和 TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 365f4c803cb7f6e7b18570534819e576990d11de
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050792"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="4d01f-103">tiIndicator：deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="4d01f-103">tiIndicator: deleteTiIndicators</span></span>

<span data-ttu-id="4d01f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d01f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d01f-105">在一个 (而不是) 个请求中删除多个威胁情报和 TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="4d01f-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d01f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4d01f-106">Permissions</span></span>

<span data-ttu-id="4d01f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d01f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d01f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d01f-109">Permission type</span></span> | <span data-ttu-id="4d01f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d01f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d01f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d01f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d01f-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4d01f-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="4d01f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d01f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d01f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d01f-114">Not supported.</span></span> |
| <span data-ttu-id="4d01f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d01f-115">Application</span></span>                            | <span data-ttu-id="4d01f-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4d01f-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d01f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d01f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="4d01f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d01f-118">Request headers</span></span>

| <span data-ttu-id="4d01f-119">名称</span><span class="sxs-lookup"><span data-stu-id="4d01f-119">Name</span></span>          | <span data-ttu-id="4d01f-120">说明</span><span class="sxs-lookup"><span data-stu-id="4d01f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d01f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d01f-121">Authorization</span></span> | <span data-ttu-id="4d01f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4d01f-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d01f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d01f-123">Request body</span></span>

<span data-ttu-id="4d01f-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4d01f-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d01f-125">参数</span><span class="sxs-lookup"><span data-stu-id="4d01f-125">Parameter</span></span>    | <span data-ttu-id="4d01f-126">类型</span><span class="sxs-lookup"><span data-stu-id="4d01f-126">Type</span></span>        | <span data-ttu-id="4d01f-127">说明</span><span class="sxs-lookup"><span data-stu-id="4d01f-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d01f-128">值</span><span class="sxs-lookup"><span data-stu-id="4d01f-128">value</span></span>|<span data-ttu-id="4d01f-129">字符串集合</span><span class="sxs-lookup"><span data-stu-id="4d01f-129">String collection</span></span>| <span data-ttu-id="4d01f-130">要删除的 tiIndicator `id` 集合。</span><span class="sxs-lookup"><span data-stu-id="4d01f-130">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="4d01f-131">响应</span><span class="sxs-lookup"><span data-stu-id="4d01f-131">Response</span></span>

<span data-ttu-id="4d01f-132">如果成功，此方法在 `200, OK` 响应正文中返回 响应代码和 [resultInfo](../resources/resultinfo.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="4d01f-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="4d01f-133">如果出现错误，此方法将返回 响应 `206 Partial Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="4d01f-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="4d01f-134">有关详细信息 [，](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) 请参阅错误。</span><span class="sxs-lookup"><span data-stu-id="4d01f-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="4d01f-135">示例</span><span class="sxs-lookup"><span data-stu-id="4d01f-135">Examples</span></span>

<span data-ttu-id="4d01f-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4d01f-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4d01f-137">请求</span><span class="sxs-lookup"><span data-stu-id="4d01f-137">Request</span></span>

<span data-ttu-id="4d01f-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d01f-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d01f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d01f-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4d01f-140">C#</span><span class="sxs-lookup"><span data-stu-id="4d01f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d01f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d01f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d01f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d01f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d01f-143">Java</span><span class="sxs-lookup"><span data-stu-id="4d01f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d01f-144">响应</span><span class="sxs-lookup"><span data-stu-id="4d01f-144">Response</span></span>

<span data-ttu-id="4d01f-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d01f-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4d01f-146">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4d01f-146">The response object shown here might be shortened for readability.</span></span>

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
      "code": 0,
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


