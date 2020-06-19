---
title: 列出 deviceConfigurationGroupAssignments
description: 列出 deviceConfigurationGroupAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81b48c6b146f235b3475ee4e77c4fbf7e1fac9c0
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792896"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="a49ea-103">列出 deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="a49ea-103">List deviceConfigurationGroupAssignments</span></span>

<span data-ttu-id="a49ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a49ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a49ea-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a49ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a49ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a49ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a49ea-107">列出[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a49ea-107">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a49ea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a49ea-108">Prerequisites</span></span>
<span data-ttu-id="a49ea-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a49ea-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a49ea-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a49ea-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a49ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a49ea-111">Permission type</span></span>|<span data-ttu-id="a49ea-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a49ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a49ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a49ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a49ea-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a49ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a49ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a49ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a49ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a49ea-116">Not supported.</span></span>|
|<span data-ttu-id="a49ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a49ea-117">Application</span></span>|<span data-ttu-id="a49ea-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a49ea-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a49ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a49ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a49ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a49ea-120">Request headers</span></span>
|<span data-ttu-id="a49ea-121">标头</span><span class="sxs-lookup"><span data-stu-id="a49ea-121">Header</span></span>|<span data-ttu-id="a49ea-122">值</span><span class="sxs-lookup"><span data-stu-id="a49ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a49ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a49ea-123">Authorization</span></span>|<span data-ttu-id="a49ea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a49ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a49ea-125">接受</span><span class="sxs-lookup"><span data-stu-id="a49ea-125">Accept</span></span>|<span data-ttu-id="a49ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a49ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a49ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a49ea-127">Request body</span></span>
<span data-ttu-id="a49ea-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a49ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a49ea-129">响应</span><span class="sxs-lookup"><span data-stu-id="a49ea-129">Response</span></span>
<span data-ttu-id="a49ea-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a49ea-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a49ea-131">示例</span><span class="sxs-lookup"><span data-stu-id="a49ea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a49ea-132">请求</span><span class="sxs-lookup"><span data-stu-id="a49ea-132">Request</span></span>
<span data-ttu-id="a49ea-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a49ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="a49ea-134">响应</span><span class="sxs-lookup"><span data-stu-id="a49ea-134">Response</span></span>
<span data-ttu-id="a49ea-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a49ea-135">Here is an example of the response.</span></span> <span data-ttu-id="a49ea-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a49ea-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a49ea-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a49ea-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```



