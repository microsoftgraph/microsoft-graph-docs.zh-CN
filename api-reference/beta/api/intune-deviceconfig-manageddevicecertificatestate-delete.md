---
title: 删除 managedDeviceCertificateState
description: 删除 managedDeviceCertificateState。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f76dcf72602067f9cf1d1c5d97b4732e07a66d48
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179135"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="c43a3-103">删除 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="c43a3-103">Delete managedDeviceCertificateState</span></span>

<span data-ttu-id="c43a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c43a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c43a3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c43a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c43a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c43a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c43a3-107">删除[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="c43a3-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c43a3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c43a3-108">Prerequisites</span></span>
<span data-ttu-id="c43a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c43a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c43a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c43a3-111">Permission type</span></span>|<span data-ttu-id="c43a3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c43a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c43a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c43a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c43a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c43a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c43a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c43a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c43a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c43a3-116">Not supported.</span></span>|
|<span data-ttu-id="c43a3-117">Application</span><span class="sxs-lookup"><span data-stu-id="c43a3-117">Application</span></span>|<span data-ttu-id="c43a3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c43a3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c43a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c43a3-119">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c43a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c43a3-120">Request headers</span></span>
|<span data-ttu-id="c43a3-121">标头</span><span class="sxs-lookup"><span data-stu-id="c43a3-121">Header</span></span>|<span data-ttu-id="c43a3-122">值</span><span class="sxs-lookup"><span data-stu-id="c43a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c43a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c43a3-123">Authorization</span></span>|<span data-ttu-id="c43a3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c43a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c43a3-125">接受</span><span class="sxs-lookup"><span data-stu-id="c43a3-125">Accept</span></span>|<span data-ttu-id="c43a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c43a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c43a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c43a3-127">Request body</span></span>
<span data-ttu-id="c43a3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c43a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c43a3-129">响应</span><span class="sxs-lookup"><span data-stu-id="c43a3-129">Response</span></span>
<span data-ttu-id="c43a3-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c43a3-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c43a3-131">示例</span><span class="sxs-lookup"><span data-stu-id="c43a3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c43a3-132">请求</span><span class="sxs-lookup"><span data-stu-id="c43a3-132">Request</span></span>
<span data-ttu-id="c43a3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c43a3-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="c43a3-134">响应</span><span class="sxs-lookup"><span data-stu-id="c43a3-134">Response</span></span>
<span data-ttu-id="c43a3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c43a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



