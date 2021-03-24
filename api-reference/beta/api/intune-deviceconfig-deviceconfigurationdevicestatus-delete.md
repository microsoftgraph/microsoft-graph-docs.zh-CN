---
title: 删除 deviceConfigurationDeviceStatus
description: 删除 deviceConfigurationDeviceStatus。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9b0e0d4caccb6d422b56626e3419c4c0ef8fc0a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131643"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="bceea-103">删除 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="bceea-103">Delete deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="bceea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bceea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bceea-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bceea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bceea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bceea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bceea-107">删除 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="bceea-107">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bceea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bceea-108">Prerequisites</span></span>
<span data-ttu-id="bceea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bceea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bceea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bceea-111">Permission type</span></span>|<span data-ttu-id="bceea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bceea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bceea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bceea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bceea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bceea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bceea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bceea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bceea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bceea-116">Not supported.</span></span>|
|<span data-ttu-id="bceea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bceea-117">Application</span></span>|<span data-ttu-id="bceea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bceea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bceea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bceea-119">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="bceea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bceea-120">Request headers</span></span>
|<span data-ttu-id="bceea-121">标头</span><span class="sxs-lookup"><span data-stu-id="bceea-121">Header</span></span>|<span data-ttu-id="bceea-122">值</span><span class="sxs-lookup"><span data-stu-id="bceea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bceea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bceea-123">Authorization</span></span>|<span data-ttu-id="bceea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bceea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bceea-125">接受</span><span class="sxs-lookup"><span data-stu-id="bceea-125">Accept</span></span>|<span data-ttu-id="bceea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bceea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bceea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bceea-127">Request body</span></span>
<span data-ttu-id="bceea-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bceea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bceea-129">响应</span><span class="sxs-lookup"><span data-stu-id="bceea-129">Response</span></span>
<span data-ttu-id="bceea-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bceea-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bceea-131">示例</span><span class="sxs-lookup"><span data-stu-id="bceea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bceea-132">请求</span><span class="sxs-lookup"><span data-stu-id="bceea-132">Request</span></span>
<span data-ttu-id="bceea-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bceea-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="bceea-134">响应</span><span class="sxs-lookup"><span data-stu-id="bceea-134">Response</span></span>
<span data-ttu-id="bceea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bceea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




