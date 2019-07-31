---
title: 'tiIndicator: deleteTiIndicators'
description: 在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 861b0ad0a476cfcc659bb20764b09d159c0ad61f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977487"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="c33cb-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="c33cb-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c33cb-104">在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="c33cb-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c33cb-105">权限</span><span class="sxs-lookup"><span data-stu-id="c33cb-105">Permissions</span></span>

<span data-ttu-id="c33cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c33cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c33cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c33cb-108">Permission type</span></span> | <span data-ttu-id="c33cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c33cb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c33cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c33cb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c33cb-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c33cb-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c33cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c33cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c33cb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c33cb-113">Not supported.</span></span> |
| <span data-ttu-id="c33cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c33cb-114">Application</span></span>                            | <span data-ttu-id="c33cb-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c33cb-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c33cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c33cb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="c33cb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c33cb-117">Request headers</span></span>

| <span data-ttu-id="c33cb-118">名称</span><span class="sxs-lookup"><span data-stu-id="c33cb-118">Name</span></span>          | <span data-ttu-id="c33cb-119">说明</span><span class="sxs-lookup"><span data-stu-id="c33cb-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c33cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c33cb-120">Authorization</span></span> | <span data-ttu-id="c33cb-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c33cb-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c33cb-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="c33cb-122">Request body</span></span>

<span data-ttu-id="c33cb-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c33cb-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c33cb-124">参数</span><span class="sxs-lookup"><span data-stu-id="c33cb-124">Parameter</span></span>    | <span data-ttu-id="c33cb-125">类型</span><span class="sxs-lookup"><span data-stu-id="c33cb-125">Type</span></span>        | <span data-ttu-id="c33cb-126">说明</span><span class="sxs-lookup"><span data-stu-id="c33cb-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c33cb-127">值</span><span class="sxs-lookup"><span data-stu-id="c33cb-127">value</span></span>|<span data-ttu-id="c33cb-128">String collection</span><span class="sxs-lookup"><span data-stu-id="c33cb-128">String collection</span></span>| <span data-ttu-id="c33cb-129">要删除的`id`tiIndicator 的集合。</span><span class="sxs-lookup"><span data-stu-id="c33cb-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="c33cb-130">响应</span><span class="sxs-lookup"><span data-stu-id="c33cb-130">Response</span></span>

<span data-ttu-id="c33cb-131">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[resultInfo](../resources/resultinfo.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="c33cb-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c33cb-132">示例</span><span class="sxs-lookup"><span data-stu-id="c33cb-132">Examples</span></span>

<span data-ttu-id="c33cb-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c33cb-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c33cb-134">请求</span><span class="sxs-lookup"><span data-stu-id="c33cb-134">Request</span></span>

<span data-ttu-id="c33cb-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c33cb-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c33cb-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c33cb-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c33cb-137">C#</span><span class="sxs-lookup"><span data-stu-id="c33cb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c33cb-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c33cb-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c33cb-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="c33cb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c33cb-140">Java</span><span class="sxs-lookup"><span data-stu-id="c33cb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c33cb-141">响应</span><span class="sxs-lookup"><span data-stu-id="c33cb-141">Response</span></span>

<span data-ttu-id="c33cb-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c33cb-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c33cb-143">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c33cb-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c33cb-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c33cb-144">All the properties will be returned from an actual call.</span></span>

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
