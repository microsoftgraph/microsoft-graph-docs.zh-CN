---
title: 删除 deviceConfigurationDeviceStatus
description: 删除 deviceConfigurationDeviceStatus。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cb807d186408d6cd76a701b5b19bdf6a94338db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792945"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="eb444-103">删除 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="eb444-103">Delete deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="eb444-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb444-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb444-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb444-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb444-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb444-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb444-107">删除 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="eb444-107">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb444-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb444-108">Prerequisites</span></span>
<span data-ttu-id="eb444-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="eb444-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="eb444-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb444-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb444-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb444-111">Permission type</span></span>|<span data-ttu-id="eb444-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb444-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb444-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb444-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb444-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb444-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb444-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb444-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb444-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb444-116">Not supported.</span></span>|
|<span data-ttu-id="eb444-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb444-117">Application</span></span>|<span data-ttu-id="eb444-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb444-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb444-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb444-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="eb444-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb444-120">Request headers</span></span>
|<span data-ttu-id="eb444-121">标头</span><span class="sxs-lookup"><span data-stu-id="eb444-121">Header</span></span>|<span data-ttu-id="eb444-122">值</span><span class="sxs-lookup"><span data-stu-id="eb444-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb444-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb444-123">Authorization</span></span>|<span data-ttu-id="eb444-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb444-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb444-125">接受</span><span class="sxs-lookup"><span data-stu-id="eb444-125">Accept</span></span>|<span data-ttu-id="eb444-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb444-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb444-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb444-127">Request body</span></span>
<span data-ttu-id="eb444-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb444-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb444-129">响应</span><span class="sxs-lookup"><span data-stu-id="eb444-129">Response</span></span>
<span data-ttu-id="eb444-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb444-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eb444-131">示例</span><span class="sxs-lookup"><span data-stu-id="eb444-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb444-132">请求</span><span class="sxs-lookup"><span data-stu-id="eb444-132">Request</span></span>
<span data-ttu-id="eb444-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb444-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="eb444-134">响应</span><span class="sxs-lookup"><span data-stu-id="eb444-134">Response</span></span>
<span data-ttu-id="eb444-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="eb444-135">Here is an example of the response.</span></span> <span data-ttu-id="eb444-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="eb444-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eb444-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="eb444-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



