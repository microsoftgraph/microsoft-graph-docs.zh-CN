---
title: 获取 raProfileDatabaseEntity
description: 读取 raProfileDatabaseEntity 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0dbd34afd108a50a5e91aac414cc19ecd86282
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124241"
---
# <a name="get-raprofiledatabaseentity"></a><span data-ttu-id="a4ad3-103">获取 raProfileDatabaseEntity</span><span class="sxs-lookup"><span data-stu-id="a4ad3-103">Get raProfileDatabaseEntity</span></span>

<span data-ttu-id="a4ad3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ad3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4ad3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4ad3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4ad3-107">读取[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-107">Read properties and relationships of the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4ad3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4ad3-108">Prerequisites</span></span>
<span data-ttu-id="a4ad3-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a4ad3-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a4ad3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ad3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ad3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4ad3-111">Permission type</span></span>|<span data-ttu-id="a4ad3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4ad3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4ad3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4ad3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4ad3-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4ad3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a4ad3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4ad3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4ad3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-116">Not supported.</span></span>|
|<span data-ttu-id="a4ad3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4ad3-117">Application</span></span>|<span data-ttu-id="a4ad3-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4ad3-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4ad3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4ad3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4ad3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4ad3-120">Optional query parameters</span></span>
<span data-ttu-id="a4ad3-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4ad3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4ad3-122">Request headers</span></span>
|<span data-ttu-id="a4ad3-123">标头</span><span class="sxs-lookup"><span data-stu-id="a4ad3-123">Header</span></span>|<span data-ttu-id="a4ad3-124">值</span><span class="sxs-lookup"><span data-stu-id="a4ad3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4ad3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ad3-125">Authorization</span></span>|<span data-ttu-id="a4ad3-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4ad3-127">接受</span><span class="sxs-lookup"><span data-stu-id="a4ad3-127">Accept</span></span>|<span data-ttu-id="a4ad3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a4ad3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ad3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4ad3-129">Request body</span></span>
<span data-ttu-id="a4ad3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4ad3-131">响应</span><span class="sxs-lookup"><span data-stu-id="a4ad3-131">Response</span></span>
<span data-ttu-id="a4ad3-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-132">If successful, this method returns a `200 OK` response code and [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ad3-133">示例</span><span class="sxs-lookup"><span data-stu-id="a4ad3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4ad3-134">请求</span><span class="sxs-lookup"><span data-stu-id="a4ad3-134">Request</span></span>
<span data-ttu-id="a4ad3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4ad3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a><span data-ttu-id="a4ad3-136">响应</span><span class="sxs-lookup"><span data-stu-id="a4ad3-136">Response</span></span>
<span data-ttu-id="a4ad3-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a4ad3-137">Here is an example of the response.</span></span> <span data-ttu-id="a4ad3-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a4ad3-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a4ad3-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a4ad3-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "value": {
    "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
    "version": 7,
    "isDeleted": true,
    "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
    "displayName": "Display Name value",
    "linkedProfileIds": [
      "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
    ],
    "profileTypeName": "Profile Type Name value",
    "profileBody": "Profile Body value",
    "profileBodyHash": "Profile Body Hash value",
    "platformType": 12,
    "transformedProfileBody": "Transformed Profile Body value",
    "transformedProfileBodyHash": "Transformed Profile Body Hash value",
    "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
    "profileId": "6389d896-d896-6389-96d8-896396d88963",
    "eTag": "ETag value",
    "schemaVersion": "betaStart",
    "lastModified": "2017-01-01T00:03:14.6651031-08:00"
  }
}
```



