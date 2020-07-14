---
title: 列出 deviceConfigurationAssignments
description: 列出 deviceConfigurationAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 264a453491fb75c52777d9e8ba5a40cfba96505f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123146"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="a3f8a-103">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="a3f8a-103">List deviceConfigurationAssignments</span></span>

<span data-ttu-id="a3f8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3f8a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3f8a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3f8a-107">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3f8a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3f8a-108">Prerequisites</span></span>
<span data-ttu-id="a3f8a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a3f8a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a3f8a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3f8a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3f8a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3f8a-111">Permission type</span></span>|<span data-ttu-id="a3f8a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a3f8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3f8a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3f8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3f8a-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3f8a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3f8a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3f8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3f8a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-116">Not supported.</span></span>|
|<span data-ttu-id="a3f8a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3f8a-117">Application</span></span>|<span data-ttu-id="a3f8a-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3f8a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3f8a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3f8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a3f8a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3f8a-120">Request headers</span></span>
|<span data-ttu-id="a3f8a-121">标头</span><span class="sxs-lookup"><span data-stu-id="a3f8a-121">Header</span></span>|<span data-ttu-id="a3f8a-122">值</span><span class="sxs-lookup"><span data-stu-id="a3f8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3f8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3f8a-123">Authorization</span></span>|<span data-ttu-id="a3f8a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3f8a-125">接受</span><span class="sxs-lookup"><span data-stu-id="a3f8a-125">Accept</span></span>|<span data-ttu-id="a3f8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3f8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3f8a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3f8a-127">Request body</span></span>
<span data-ttu-id="a3f8a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3f8a-129">响应</span><span class="sxs-lookup"><span data-stu-id="a3f8a-129">Response</span></span>
<span data-ttu-id="a3f8a-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3f8a-131">示例</span><span class="sxs-lookup"><span data-stu-id="a3f8a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3f8a-132">请求</span><span class="sxs-lookup"><span data-stu-id="a3f8a-132">Request</span></span>
<span data-ttu-id="a3f8a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3f8a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="a3f8a-134">响应</span><span class="sxs-lookup"><span data-stu-id="a3f8a-134">Response</span></span>
<span data-ttu-id="a3f8a-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a3f8a-135">Here is an example of the response.</span></span> <span data-ttu-id="a3f8a-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a3f8a-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3f8a-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a3f8a-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



