---
title: 获取历史记录
description: 读取 riskyUserHistoryItem 对象的属性和关系。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 141aaa6a1c0642159cccfe075aa8934fa65883cd
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897573"
---
# <a name="get-history"></a><span data-ttu-id="9c0a4-103">获取历史记录</span><span class="sxs-lookup"><span data-stu-id="9c0a4-103">Get history</span></span>
<span data-ttu-id="9c0a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c0a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c0a4-105">读取[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-105">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>


><span data-ttu-id="9c0a4-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c0a4-107">权限</span><span class="sxs-lookup"><span data-stu-id="9c0a4-107">Permissions</span></span>
<span data-ttu-id="9c0a4-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9c0a4-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9c0a4-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="9c0a4-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="9c0a4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c0a4-110">Permission type</span></span>      | <span data-ttu-id="9c0a4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c0a4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c0a4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c0a4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c0a4-113">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="9c0a4-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c0a4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c0a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c0a4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-115">Not supported.</span></span>    |
|<span data-ttu-id="9c0a4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c0a4-116">Application</span></span> | <span data-ttu-id="9c0a4-117">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="9c0a4-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c0a4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c0a4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{userId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c0a4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9c0a4-119">Optional query parameters</span></span>
<span data-ttu-id="9c0a4-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9c0a4-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c0a4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c0a4-122">Request headers</span></span>
|<span data-ttu-id="9c0a4-123">名称</span><span class="sxs-lookup"><span data-stu-id="9c0a4-123">Name</span></span>|<span data-ttu-id="9c0a4-124">说明</span><span class="sxs-lookup"><span data-stu-id="9c0a4-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9c0a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c0a4-125">Authorization</span></span>|<span data-ttu-id="9c0a4-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="9c0a4-126">Bearer {token}.</span></span> <span data-ttu-id="9c0a4-127">Required.</span><span class="sxs-lookup"><span data-stu-id="9c0a4-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c0a4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c0a4-128">Request body</span></span>
<span data-ttu-id="9c0a4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c0a4-130">响应</span><span class="sxs-lookup"><span data-stu-id="9c0a4-130">Response</span></span>

<span data-ttu-id="9c0a4-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-131">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c0a4-132">示例</span><span class="sxs-lookup"><span data-stu-id="9c0a4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c0a4-133">请求</span><span class="sxs-lookup"><span data-stu-id="9c0a4-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```


### <a name="response"></a><span data-ttu-id="9c0a4-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c0a4-134">Response</span></span>
<span data-ttu-id="9c0a4-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9c0a4-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": 
  {
    "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
      "@odata.type": "microsoft.graph.riskUserActivity"
    }
  }
}
```

