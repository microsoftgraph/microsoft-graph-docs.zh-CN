---
title: 删除 managedDeviceCertificateState
description: 删除 managedDeviceCertificateState。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: beb1af20c72e44659bc1fb044b717c475992dd8b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37183651"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="18697-103">删除 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="18697-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="18697-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18697-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18697-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18697-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18697-106">删除[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="18697-106">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18697-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="18697-107">Prerequisites</span></span>
<span data-ttu-id="18697-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18697-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="18697-110">Permission type</span></span>|<span data-ttu-id="18697-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18697-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18697-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18697-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18697-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18697-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18697-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18697-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18697-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="18697-115">Not supported.</span></span>|
|<span data-ttu-id="18697-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="18697-116">Application</span></span>|<span data-ttu-id="18697-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18697-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18697-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18697-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="18697-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="18697-119">Request headers</span></span>
|<span data-ttu-id="18697-120">标头</span><span class="sxs-lookup"><span data-stu-id="18697-120">Header</span></span>|<span data-ttu-id="18697-121">值</span><span class="sxs-lookup"><span data-stu-id="18697-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18697-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18697-122">Authorization</span></span>|<span data-ttu-id="18697-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18697-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18697-124">接受</span><span class="sxs-lookup"><span data-stu-id="18697-124">Accept</span></span>|<span data-ttu-id="18697-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18697-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18697-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18697-126">Request body</span></span>
<span data-ttu-id="18697-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18697-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18697-128">响应</span><span class="sxs-lookup"><span data-stu-id="18697-128">Response</span></span>
<span data-ttu-id="18697-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18697-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18697-130">示例</span><span class="sxs-lookup"><span data-stu-id="18697-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="18697-131">请求</span><span class="sxs-lookup"><span data-stu-id="18697-131">Request</span></span>
<span data-ttu-id="18697-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18697-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="18697-133">响应</span><span class="sxs-lookup"><span data-stu-id="18697-133">Response</span></span>
<span data-ttu-id="18697-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18697-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




