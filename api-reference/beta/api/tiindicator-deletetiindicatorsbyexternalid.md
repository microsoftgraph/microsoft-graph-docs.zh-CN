---
title: tiIndicator：deleteTiIndicatorsByExternalId
description: 在一个 (（) 个请求）中删除多个威胁情报和 TI) 指示器，并且请求包含外部 ID 而不是 ID。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a163f2c2a362cda42964733bf6639a2138dcb98c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052661"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="99909-103">tiIndicator：deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="99909-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

<span data-ttu-id="99909-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99909-105">当请求包含外部 (（而不是) ）时，在一个请求（而不是多个请求）中删除多个威胁情报和 TI 智能指示器。</span><span class="sxs-lookup"><span data-stu-id="99909-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="99909-106">权限</span><span class="sxs-lookup"><span data-stu-id="99909-106">Permissions</span></span>

<span data-ttu-id="99909-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99909-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99909-109">Permission type</span></span>  | <span data-ttu-id="99909-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99909-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99909-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99909-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="99909-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="99909-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="99909-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99909-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99909-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99909-114">Not supported.</span></span> |
| <span data-ttu-id="99909-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99909-115">Application</span></span>                            | <span data-ttu-id="99909-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="99909-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="99909-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99909-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="99909-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="99909-118">Request headers</span></span>

| <span data-ttu-id="99909-119">名称</span><span class="sxs-lookup"><span data-stu-id="99909-119">Name</span></span>          | <span data-ttu-id="99909-120">说明</span><span class="sxs-lookup"><span data-stu-id="99909-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="99909-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="99909-121">Authorization</span></span> | <span data-ttu-id="99909-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="99909-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="99909-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="99909-123">Request body</span></span>

<span data-ttu-id="99909-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="99909-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99909-125">参数</span><span class="sxs-lookup"><span data-stu-id="99909-125">Parameter</span></span>    | <span data-ttu-id="99909-126">类型</span><span class="sxs-lookup"><span data-stu-id="99909-126">Type</span></span>        | <span data-ttu-id="99909-127">说明</span><span class="sxs-lookup"><span data-stu-id="99909-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99909-128">值</span><span class="sxs-lookup"><span data-stu-id="99909-128">value</span></span>|<span data-ttu-id="99909-129">字符串集合</span><span class="sxs-lookup"><span data-stu-id="99909-129">String collection</span></span>| <span data-ttu-id="99909-130">要 `externalIds` 删除的 **tiIndicator** 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="99909-130">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="99909-131">响应</span><span class="sxs-lookup"><span data-stu-id="99909-131">Response</span></span>

<span data-ttu-id="99909-132">如果成功，此方法在 `200, OK` 响应正文中返回 响应代码和 [resultInfo](../resources/resultinfo.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="99909-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="99909-133">如果出现错误，此方法将返回 响应 `206 Partial Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="99909-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="99909-134">有关详细信息 [，](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) 请参阅错误。</span><span class="sxs-lookup"><span data-stu-id="99909-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="99909-135">示例</span><span class="sxs-lookup"><span data-stu-id="99909-135">Examples</span></span>

<span data-ttu-id="99909-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="99909-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="99909-137">请求</span><span class="sxs-lookup"><span data-stu-id="99909-137">Request</span></span>

<span data-ttu-id="99909-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99909-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99909-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="99909-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="99909-140">C#</span><span class="sxs-lookup"><span data-stu-id="99909-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicatorsbyexternalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99909-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99909-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicatorsbyexternalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99909-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99909-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicatorsbyexternalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99909-143">Java</span><span class="sxs-lookup"><span data-stu-id="99909-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicatorsbyexternalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99909-144">响应</span><span class="sxs-lookup"><span data-stu-id="99909-144">Response</span></span>

<span data-ttu-id="99909-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99909-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="99909-146">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99909-146">The response object shown here might be shortened for readability.</span></span>

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
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


