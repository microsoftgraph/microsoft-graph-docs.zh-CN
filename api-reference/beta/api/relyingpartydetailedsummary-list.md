---
title: 列出 relyingPartyDetailedSummary
description: 检索 relyingPartyDetailedSummary 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc7b05e012507cc1e6e36cf3ee189f6b63100d4d
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543453"
---
# <a name="list-relyingpartydetailedsummary"></a><span data-ttu-id="0ad71-103">列出 relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="0ad71-103">List relyingPartyDetailedSummary</span></span>

<span data-ttu-id="0ad71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ad71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad71-105">检索**relyingPartyDetailedSummary**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0ad71-105">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ad71-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ad71-106">Permissions</span></span>

<span data-ttu-id="0ad71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ad71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ad71-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ad71-109">Permission type</span></span>                        | <span data-ttu-id="0ad71-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ad71-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ad71-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ad71-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ad71-112">Report. All</span><span class="sxs-lookup"><span data-stu-id="0ad71-112">Report.Read.All</span></span> |
| <span data-ttu-id="0ad71-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ad71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ad71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ad71-114">Not supported.</span></span> |
| <span data-ttu-id="0ad71-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ad71-115">Application</span></span>                            | <span data-ttu-id="0ad71-116">Report. All</span><span class="sxs-lookup"><span data-stu-id="0ad71-116">Report.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ad71-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ad71-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getRelyingPartyDetailedSummary
```
## <a name="function-parameters"></a><span data-ttu-id="0ad71-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="0ad71-118">Function parameters</span></span>

| <span data-ttu-id="0ad71-119">参数</span><span class="sxs-lookup"><span data-stu-id="0ad71-119">Parameter</span></span> | <span data-ttu-id="0ad71-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ad71-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0ad71-121">period</span><span class="sxs-lookup"><span data-stu-id="0ad71-121">period</span></span> | <span data-ttu-id="0ad71-122">受支持的值为： D1、D7、D30。</span><span class="sxs-lookup"><span data-stu-id="0ad71-122">The supported values are: D1, D7, D30.</span></span> <span data-ttu-id="0ad71-123">这些值采用格式 Dn，其中 n 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0ad71-123">These values follow the format Dn where n represents the number of days over which the report is aggregated.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="0ad71-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ad71-124">Optional query parameters</span></span>

<span data-ttu-id="0ad71-125">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ad71-125">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="0ad71-126">您可以使用`$filter`参数按 RelyingPartyId、migrationStatus 和其他属性进行筛选。</span><span class="sxs-lookup"><span data-stu-id="0ad71-126">You can use the `$filter` parameter to filter by relyingPartyId, migrationStatus and other attributes.</span></span> <span data-ttu-id="0ad71-127">例如，$filter = relyingPartyId eq ' 标识符 '。</span><span class="sxs-lookup"><span data-stu-id="0ad71-127">For example, $filter= relyingPartyId eq 'identifier'.</span></span>
- <span data-ttu-id="0ad71-128">可以在任何`$orderby`GET `$top`请求中`$skip`使用、和查询参数。</span><span class="sxs-lookup"><span data-stu-id="0ad71-128">You can use `$orderby`, `$top`, and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="0ad71-129">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0ad71-129">For general information, see [OData query parameters](/graph/query-parameters).</span></span>


## <a name="request-headers"></a><span data-ttu-id="0ad71-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ad71-130">Request headers</span></span>

| <span data-ttu-id="0ad71-131">名称</span><span class="sxs-lookup"><span data-stu-id="0ad71-131">Name</span></span>      |<span data-ttu-id="0ad71-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ad71-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ad71-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ad71-133">Authorization</span></span> | <span data-ttu-id="0ad71-134">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="0ad71-134">Bearer {code}.</span></span> <span data-ttu-id="0ad71-135">必需。</span><span class="sxs-lookup"><span data-stu-id="0ad71-135">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ad71-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ad71-136">Request body</span></span>

<span data-ttu-id="0ad71-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ad71-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ad71-138">响应</span><span class="sxs-lookup"><span data-stu-id="0ad71-138">Response</span></span>

<span data-ttu-id="0ad71-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ad71-139">If successful, this method returns a `200 OK` response code and the requested [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ad71-140">示例</span><span class="sxs-lookup"><span data-stu-id="0ad71-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ad71-141">请求</span><span class="sxs-lookup"><span data-stu-id="0ad71-141">Request</span></span>

<span data-ttu-id="0ad71-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ad71-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='period_value')
```

### <a name="response"></a><span data-ttu-id="0ad71-143">响应</span><span class="sxs-lookup"><span data-stu-id="0ad71-143">Response</span></span>

<span data-ttu-id="0ad71-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ad71-144">The following is an example of the response.</span></span>

> <span data-ttu-id="0ad71-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ad71-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1fec2821-6c43-4919-9560-ce36c820faa5",
  "relyingPartyId": "https://contosoorg-dev-ed.my.contoso.com",
  "serviceId": "287ed092-c182-4748-99a9-9ef3b5a0a0f9",
  "relyingPartyName": "contoso",
  "successfulSignInCount": 90,
  "failedSignInCount": 10,
  "totalSignInCount": 100,
  "signInSuccessRate":90.0,
  "uniqueUserCount": 10,
  "migrationStatus": "ready",
  "replyUrls": [
      "https://contosoorg-dev-ed.my.contoso.com"
  ],
  "migrationValidationDetails": [
      {
          "name": "AdditionalWSFedEndpointCheckResult",
          "value": "{\"result\": 0, \"message\": \"No additional WS-Federation endpoints were found.\"}"
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get relyingPartyDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
