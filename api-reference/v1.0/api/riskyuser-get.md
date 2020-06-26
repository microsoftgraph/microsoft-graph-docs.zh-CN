---
title: 获取 riskyUser
description: 读取 riskyUser 对象的属性和关系。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb017f25388a75157a5050b0a08049b075d67ab0
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897566"
---
# <a name="get-riskyuser"></a><span data-ttu-id="239dd-103">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="239dd-103">Get riskyUser</span></span>
<span data-ttu-id="239dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="239dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="239dd-105">读取[riskyUser](../resources/riskyuser.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="239dd-105">Read the properties and relationships of a [riskyUser](../resources/riskyuser.md) object.</span></span>

><span data-ttu-id="239dd-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="239dd-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="239dd-107">权限</span><span class="sxs-lookup"><span data-stu-id="239dd-107">Permissions</span></span>
<span data-ttu-id="239dd-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="239dd-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="239dd-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="239dd-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="239dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="239dd-110">Permission type</span></span>      | <span data-ttu-id="239dd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="239dd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="239dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="239dd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="239dd-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="239dd-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="239dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="239dd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="239dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="239dd-115">Not supported.</span></span>    |
|<span data-ttu-id="239dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="239dd-116">Application</span></span> | <span data-ttu-id="239dd-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="239dd-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="239dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="239dd-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="239dd-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="239dd-119">Optional query parameters</span></span>
<span data-ttu-id="239dd-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="239dd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="239dd-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="239dd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="239dd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="239dd-122">Request headers</span></span>
|<span data-ttu-id="239dd-123">名称</span><span class="sxs-lookup"><span data-stu-id="239dd-123">Name</span></span>|<span data-ttu-id="239dd-124">说明</span><span class="sxs-lookup"><span data-stu-id="239dd-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="239dd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="239dd-125">Authorization</span></span>|<span data-ttu-id="239dd-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="239dd-126">Bearer {token}.</span></span> <span data-ttu-id="239dd-127">Required.</span><span class="sxs-lookup"><span data-stu-id="239dd-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="239dd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="239dd-128">Request body</span></span>
<span data-ttu-id="239dd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="239dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="239dd-130">响应</span><span class="sxs-lookup"><span data-stu-id="239dd-130">Response</span></span>

<span data-ttu-id="239dd-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="239dd-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="239dd-132">示例</span><span class="sxs-lookup"><span data-stu-id="239dd-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="239dd-133">请求</span><span class="sxs-lookup"><span data-stu-id="239dd-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```


### <a name="response"></a><span data-ttu-id="239dd-134">响应</span><span class="sxs-lookup"><span data-stu-id="239dd-134">Response</span></span>
<span data-ttu-id="239dd-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="239dd-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUser",
      "id": "d1d4a5d4-a5d4-d1d4-d4a5-d4d1d4a5d4d1",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String"
    }
  ]
}
```

