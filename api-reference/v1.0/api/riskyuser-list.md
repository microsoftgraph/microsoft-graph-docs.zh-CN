---
title: 列出 riskyUsers
description: 获取 riskyUser 对象及其属性的列表。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd6d413803e7461ffe0f00891b6e4db7cd3d0e0b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897552"
---
# <a name="list-riskyusers"></a><span data-ttu-id="ee926-103">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ee926-103">List riskyUsers</span></span>
<span data-ttu-id="ee926-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee926-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee926-105">获取[riskyUser](../resources/riskyuser.md)对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="ee926-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee926-106">权限</span><span class="sxs-lookup"><span data-stu-id="ee926-106">Permissions</span></span>
<span data-ttu-id="ee926-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ee926-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ee926-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="ee926-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="ee926-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee926-109">Permission type</span></span>|<span data-ttu-id="ee926-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ee926-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee926-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee926-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee926-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee926-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="ee926-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee926-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee926-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee926-114">Not supported.</span></span>    |
|<span data-ttu-id="ee926-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee926-115">Application</span></span> | <span data-ttu-id="ee926-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee926-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee926-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee926-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee926-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ee926-118">Optional query parameters</span></span>
<span data-ttu-id="ee926-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ee926-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee926-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ee926-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee926-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee926-121">Request headers</span></span>
|<span data-ttu-id="ee926-122">名称</span><span class="sxs-lookup"><span data-stu-id="ee926-122">Name</span></span>|<span data-ttu-id="ee926-123">说明</span><span class="sxs-lookup"><span data-stu-id="ee926-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee926-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee926-124">Authorization</span></span>|<span data-ttu-id="ee926-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ee926-125">Bearer {token}.</span></span> <span data-ttu-id="ee926-126">Required.</span><span class="sxs-lookup"><span data-stu-id="ee926-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee926-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee926-127">Request body</span></span>
<span data-ttu-id="ee926-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee926-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee926-129">响应</span><span class="sxs-lookup"><span data-stu-id="ee926-129">Response</span></span>

<span data-ttu-id="ee926-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ee926-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee926-131">示例</span><span class="sxs-lookup"><span data-stu-id="ee926-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee926-132">请求</span><span class="sxs-lookup"><span data-stu-id="ee926-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="ee926-133">响应</span><span class="sxs-lookup"><span data-stu-id="ee926-133">Response</span></span>
<span data-ttu-id="ee926-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee926-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUser)"
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

