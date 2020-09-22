---
title: 列表历史记录
description: 从 "历史记录" 导航属性中获取 riskyUserHistoryItems。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1fcbe019d1aa673d100cedf5904b529960cec9b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051331"
---
# <a name="list-history"></a><span data-ttu-id="f0699-103">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="f0699-103">List history</span></span>
<span data-ttu-id="f0699-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0699-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0699-105">从 "历史记录" 导航属性中获取 riskyUserHistoryItems。</span><span class="sxs-lookup"><span data-stu-id="f0699-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0699-106">权限</span><span class="sxs-lookup"><span data-stu-id="f0699-106">Permissions</span></span>
<span data-ttu-id="f0699-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="f0699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="f0699-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0699-109">Permission type</span></span>|<span data-ttu-id="f0699-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0699-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0699-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0699-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0699-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0699-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="f0699-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0699-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0699-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0699-114">Not supported.</span></span>    |
|<span data-ttu-id="f0699-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0699-115">Application</span></span> | <span data-ttu-id="f0699-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0699-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0699-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0699-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0699-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0699-118">Optional query parameters</span></span>
<span data-ttu-id="f0699-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0699-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f0699-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f0699-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0699-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0699-121">Request headers</span></span>
|<span data-ttu-id="f0699-122">名称</span><span class="sxs-lookup"><span data-stu-id="f0699-122">Name</span></span>|<span data-ttu-id="f0699-123">说明</span><span class="sxs-lookup"><span data-stu-id="f0699-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f0699-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0699-124">Authorization</span></span>|<span data-ttu-id="f0699-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0699-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0699-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0699-127">Request body</span></span>
<span data-ttu-id="f0699-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0699-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0699-129">响应</span><span class="sxs-lookup"><span data-stu-id="f0699-129">Response</span></span>

<span data-ttu-id="f0699-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f0699-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0699-131">示例</span><span class="sxs-lookup"><span data-stu-id="f0699-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0699-132">请求</span><span class="sxs-lookup"><span data-stu-id="f0699-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="f0699-133">响应</span><span class="sxs-lookup"><span data-stu-id="f0699-133">Response</span></span>
<span data-ttu-id="f0699-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0699-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUserHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "5e1d812e-812e-5e1d-2e81-1d5e2e811d5e",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userId": "String",
      "initiatedBy": "String",
      "activity": {
          "riskEventTypes": [],
          "detail": "userPerformedSecuredPasswordReset"
      }
    }
  ]
}
```


