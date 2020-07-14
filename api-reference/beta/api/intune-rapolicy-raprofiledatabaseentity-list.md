---
title: 列出 raProfileDatabaseEntities
description: 列出 raProfileDatabaseEntity 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca8a822b0a79d1e9144261b6cd2f219ee01cbcbb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124240"
---
# <a name="list-raprofiledatabaseentities"></a><span data-ttu-id="f9dfa-103">列出 raProfileDatabaseEntities</span><span class="sxs-lookup"><span data-stu-id="f9dfa-103">List raProfileDatabaseEntities</span></span>

<span data-ttu-id="f9dfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9dfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9dfa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9dfa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9dfa-107">列出[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-107">List properties and relationships of the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9dfa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9dfa-108">Prerequisites</span></span>
<span data-ttu-id="f9dfa-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f9dfa-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f9dfa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9dfa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9dfa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9dfa-111">Permission type</span></span>|<span data-ttu-id="f9dfa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9dfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9dfa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9dfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9dfa-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9dfa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f9dfa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9dfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9dfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-116">Not supported.</span></span>|
|<span data-ttu-id="f9dfa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9dfa-117">Application</span></span>|<span data-ttu-id="f9dfa-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9dfa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9dfa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9dfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities
```

## <a name="request-headers"></a><span data-ttu-id="f9dfa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9dfa-120">Request headers</span></span>
|<span data-ttu-id="f9dfa-121">标头</span><span class="sxs-lookup"><span data-stu-id="f9dfa-121">Header</span></span>|<span data-ttu-id="f9dfa-122">值</span><span class="sxs-lookup"><span data-stu-id="f9dfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9dfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9dfa-123">Authorization</span></span>|<span data-ttu-id="f9dfa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9dfa-125">接受</span><span class="sxs-lookup"><span data-stu-id="f9dfa-125">Accept</span></span>|<span data-ttu-id="f9dfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9dfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9dfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9dfa-127">Request body</span></span>
<span data-ttu-id="f9dfa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9dfa-129">响应</span><span class="sxs-lookup"><span data-stu-id="f9dfa-129">Response</span></span>
<span data-ttu-id="f9dfa-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-130">If successful, this method returns a `200 OK` response code and a collection of [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9dfa-131">示例</span><span class="sxs-lookup"><span data-stu-id="f9dfa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9dfa-132">请求</span><span class="sxs-lookup"><span data-stu-id="f9dfa-132">Request</span></span>
<span data-ttu-id="f9dfa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9dfa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities
```

### <a name="response"></a><span data-ttu-id="f9dfa-134">响应</span><span class="sxs-lookup"><span data-stu-id="f9dfa-134">Response</span></span>
<span data-ttu-id="f9dfa-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f9dfa-135">Here is an example of the response.</span></span> <span data-ttu-id="f9dfa-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f9dfa-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f9dfa-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f9dfa-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": [
    {
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
  ]
}
```



