---
title: 'tiIndicator: deleteTiIndicators'
description: 在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 49475f15520f02cc36bb1bf37af9a5849a8ee245
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544656"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="62da6-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="62da6-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62da6-104">在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="62da6-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="62da6-105">权限</span><span class="sxs-lookup"><span data-stu-id="62da6-105">Permissions</span></span>

<span data-ttu-id="62da6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62da6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62da6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="62da6-108">Permission type</span></span> | <span data-ttu-id="62da6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62da6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62da6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62da6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62da6-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="62da6-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="62da6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62da6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62da6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="62da6-113">Not supported.</span></span> |
| <span data-ttu-id="62da6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="62da6-114">Application</span></span>                            | <span data-ttu-id="62da6-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="62da6-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="62da6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62da6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="62da6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="62da6-117">Request headers</span></span>

| <span data-ttu-id="62da6-118">名称</span><span class="sxs-lookup"><span data-stu-id="62da6-118">Name</span></span>          | <span data-ttu-id="62da6-119">说明</span><span class="sxs-lookup"><span data-stu-id="62da6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="62da6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="62da6-120">Authorization</span></span> | <span data-ttu-id="62da6-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="62da6-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="62da6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="62da6-122">Request body</span></span>

<span data-ttu-id="62da6-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="62da6-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62da6-124">参数</span><span class="sxs-lookup"><span data-stu-id="62da6-124">Parameter</span></span>    | <span data-ttu-id="62da6-125">类型</span><span class="sxs-lookup"><span data-stu-id="62da6-125">Type</span></span>        | <span data-ttu-id="62da6-126">说明</span><span class="sxs-lookup"><span data-stu-id="62da6-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62da6-127">值</span><span class="sxs-lookup"><span data-stu-id="62da6-127">value</span></span>|<span data-ttu-id="62da6-128">String collection</span><span class="sxs-lookup"><span data-stu-id="62da6-128">String collection</span></span>| <span data-ttu-id="62da6-129">要删除的`id`tiIndicator 的集合。</span><span class="sxs-lookup"><span data-stu-id="62da6-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="62da6-130">响应</span><span class="sxs-lookup"><span data-stu-id="62da6-130">Response</span></span>

<span data-ttu-id="62da6-131">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[resultInfo](../resources/resultinfo.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="62da6-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62da6-132">示例</span><span class="sxs-lookup"><span data-stu-id="62da6-132">Examples</span></span>

<span data-ttu-id="62da6-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="62da6-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="62da6-134">请求</span><span class="sxs-lookup"><span data-stu-id="62da6-134">Request</span></span>

<span data-ttu-id="62da6-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62da6-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62da6-136">响应</span><span class="sxs-lookup"><span data-stu-id="62da6-136">Response</span></span>

<span data-ttu-id="62da6-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62da6-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="62da6-138">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62da6-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="62da6-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62da6-139">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
