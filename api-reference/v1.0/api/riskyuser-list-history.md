---
title: 列表历史记录
description: 从 "历史记录" 导航属性中获取 riskyUserHistoryItems。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 212f10e5794a55dec925d1ec32c37abf9708700b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897559"
---
# <a name="list-history"></a><span data-ttu-id="9a251-103">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="9a251-103">List history</span></span>
<span data-ttu-id="9a251-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a251-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a251-105">从 "历史记录" 导航属性中获取 riskyUserHistoryItems。</span><span class="sxs-lookup"><span data-stu-id="9a251-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a251-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a251-106">Permissions</span></span>
<span data-ttu-id="9a251-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9a251-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9a251-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="9a251-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="9a251-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a251-109">Permission type</span></span>|<span data-ttu-id="9a251-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a251-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a251-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a251-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a251-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a251-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="9a251-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a251-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a251-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a251-114">Not supported.</span></span>    |
|<span data-ttu-id="9a251-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a251-115">Application</span></span> | <span data-ttu-id="9a251-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a251-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a251-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a251-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a251-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a251-118">Optional query parameters</span></span>
<span data-ttu-id="9a251-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9a251-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9a251-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9a251-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a251-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a251-121">Request headers</span></span>
|<span data-ttu-id="9a251-122">名称</span><span class="sxs-lookup"><span data-stu-id="9a251-122">Name</span></span>|<span data-ttu-id="9a251-123">说明</span><span class="sxs-lookup"><span data-stu-id="9a251-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9a251-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a251-124">Authorization</span></span>|<span data-ttu-id="9a251-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="9a251-125">Bearer {token}.</span></span> <span data-ttu-id="9a251-126">Required.</span><span class="sxs-lookup"><span data-stu-id="9a251-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a251-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a251-127">Request body</span></span>
<span data-ttu-id="9a251-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a251-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a251-129">响应</span><span class="sxs-lookup"><span data-stu-id="9a251-129">Response</span></span>

<span data-ttu-id="9a251-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9a251-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a251-131">示例</span><span class="sxs-lookup"><span data-stu-id="9a251-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a251-132">请求</span><span class="sxs-lookup"><span data-stu-id="9a251-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="9a251-133">响应</span><span class="sxs-lookup"><span data-stu-id="9a251-133">Response</span></span>
<span data-ttu-id="9a251-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a251-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

