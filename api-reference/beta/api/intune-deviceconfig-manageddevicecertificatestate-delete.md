---
title: 删除 managedDeviceCertificateState
description: 删除 managedDeviceCertificateState。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c0dfaa4d8afa55897dd3343172f643aa3ee0165
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625486"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="b0cb0-103">删除 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="b0cb0-103">Delete managedDeviceCertificateState</span></span>

<span data-ttu-id="b0cb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0cb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0cb0-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0cb0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0cb0-107">删除 [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0cb0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0cb0-108">Prerequisites</span></span>
<span data-ttu-id="b0cb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0cb0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0cb0-111">Permission type</span></span>|<span data-ttu-id="b0cb0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0cb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0cb0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0cb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0cb0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cb0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0cb0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0cb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0cb0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-116">Not supported.</span></span>|
|<span data-ttu-id="b0cb0-117">Application</span><span class="sxs-lookup"><span data-stu-id="b0cb0-117">Application</span></span>|<span data-ttu-id="b0cb0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cb0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0cb0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0cb0-119">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b0cb0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0cb0-120">Request headers</span></span>
|<span data-ttu-id="b0cb0-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0cb0-121">Header</span></span>|<span data-ttu-id="b0cb0-122">值</span><span class="sxs-lookup"><span data-stu-id="b0cb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0cb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0cb0-123">Authorization</span></span>|<span data-ttu-id="b0cb0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0cb0-125">接受</span><span class="sxs-lookup"><span data-stu-id="b0cb0-125">Accept</span></span>|<span data-ttu-id="b0cb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0cb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0cb0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0cb0-127">Request body</span></span>
<span data-ttu-id="b0cb0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0cb0-129">响应</span><span class="sxs-lookup"><span data-stu-id="b0cb0-129">Response</span></span>
<span data-ttu-id="b0cb0-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0cb0-131">示例</span><span class="sxs-lookup"><span data-stu-id="b0cb0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0cb0-132">请求</span><span class="sxs-lookup"><span data-stu-id="b0cb0-132">Request</span></span>
<span data-ttu-id="b0cb0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="b0cb0-134">响应</span><span class="sxs-lookup"><span data-stu-id="b0cb0-134">Response</span></span>
<span data-ttu-id="b0cb0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




