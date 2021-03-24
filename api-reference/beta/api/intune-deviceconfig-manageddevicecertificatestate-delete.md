---
title: 删除 managedDeviceCertificateState
description: 删除 managedDeviceCertificateState。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 172009471776d21be59f67a79b625010b60c3424
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132553"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="3ecca-103">删除 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="3ecca-103">Delete managedDeviceCertificateState</span></span>

<span data-ttu-id="3ecca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ecca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ecca-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ecca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ecca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ecca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ecca-107">删除 [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="3ecca-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ecca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ecca-108">Prerequisites</span></span>
<span data-ttu-id="3ecca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ecca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ecca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ecca-111">Permission type</span></span>|<span data-ttu-id="3ecca-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ecca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ecca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ecca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ecca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ecca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ecca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ecca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ecca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ecca-116">Not supported.</span></span>|
|<span data-ttu-id="3ecca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ecca-117">Application</span></span>|<span data-ttu-id="3ecca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ecca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ecca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ecca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3ecca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ecca-120">Request headers</span></span>
|<span data-ttu-id="3ecca-121">标头</span><span class="sxs-lookup"><span data-stu-id="3ecca-121">Header</span></span>|<span data-ttu-id="3ecca-122">值</span><span class="sxs-lookup"><span data-stu-id="3ecca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ecca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ecca-123">Authorization</span></span>|<span data-ttu-id="3ecca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ecca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ecca-125">接受</span><span class="sxs-lookup"><span data-stu-id="3ecca-125">Accept</span></span>|<span data-ttu-id="3ecca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ecca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ecca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ecca-127">Request body</span></span>
<span data-ttu-id="3ecca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ecca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ecca-129">响应</span><span class="sxs-lookup"><span data-stu-id="3ecca-129">Response</span></span>
<span data-ttu-id="3ecca-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3ecca-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ecca-131">示例</span><span class="sxs-lookup"><span data-stu-id="3ecca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ecca-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ecca-132">Request</span></span>
<span data-ttu-id="3ecca-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ecca-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="3ecca-134">响应</span><span class="sxs-lookup"><span data-stu-id="3ecca-134">Response</span></span>
<span data-ttu-id="3ecca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ecca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




