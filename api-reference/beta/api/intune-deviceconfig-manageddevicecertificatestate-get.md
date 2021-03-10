---
title: 获取 managedDeviceCertificateState
description: 读取 managedDeviceCertificateState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01d51d11c94dad0a958fef789e3a742fa5c9d649
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626017"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="e7abe-103">获取 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e7abe-103">Get managedDeviceCertificateState</span></span>

<span data-ttu-id="e7abe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7abe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7abe-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7abe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7abe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7abe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7abe-107">读取 [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7abe-107">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7abe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7abe-108">Prerequisites</span></span>
<span data-ttu-id="e7abe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7abe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7abe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7abe-111">Permission type</span></span>|<span data-ttu-id="e7abe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7abe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7abe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7abe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7abe-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7abe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7abe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7abe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7abe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7abe-116">Not supported.</span></span>|
|<span data-ttu-id="e7abe-117">Application</span><span class="sxs-lookup"><span data-stu-id="e7abe-117">Application</span></span>|<span data-ttu-id="e7abe-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7abe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7abe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7abe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7abe-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e7abe-120">Optional query parameters</span></span>
<span data-ttu-id="e7abe-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e7abe-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7abe-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7abe-122">Request headers</span></span>
|<span data-ttu-id="e7abe-123">标头</span><span class="sxs-lookup"><span data-stu-id="e7abe-123">Header</span></span>|<span data-ttu-id="e7abe-124">值</span><span class="sxs-lookup"><span data-stu-id="e7abe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7abe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7abe-125">Authorization</span></span>|<span data-ttu-id="e7abe-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7abe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7abe-127">接受</span><span class="sxs-lookup"><span data-stu-id="e7abe-127">Accept</span></span>|<span data-ttu-id="e7abe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e7abe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7abe-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7abe-129">Request body</span></span>
<span data-ttu-id="e7abe-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e7abe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7abe-131">响应</span><span class="sxs-lookup"><span data-stu-id="e7abe-131">Response</span></span>
<span data-ttu-id="e7abe-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7abe-132">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7abe-133">示例</span><span class="sxs-lookup"><span data-stu-id="e7abe-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7abe-134">请求</span><span class="sxs-lookup"><span data-stu-id="e7abe-134">Request</span></span>
<span data-ttu-id="e7abe-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7abe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="e7abe-136">响应</span><span class="sxs-lookup"><span data-stu-id="e7abe-136">Response</span></span>
<span data-ttu-id="e7abe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7abe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1637

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
    "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
    "devicePlatform": "androidForWork",
    "certificateKeyUsage": "digitalSignature",
    "certificateValidityPeriodUnits": "months",
    "certificateIssuanceState": "challengeIssued",
    "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
    "certificateSubjectNameFormat": "commonNameIncludingEmail",
    "certificateSubjectAlternativeNameFormat": "emailAddress",
    "certificateRevokeStatus": "pending",
    "certificateProfileDisplayName": "Certificate Profile Display Name value",
    "deviceDisplayName": "Device Display Name value",
    "userDisplayName": "User Display Name value",
    "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
    "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
    "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
    "certificateIssuer": "Certificate Issuer value",
    "certificateThumbprint": "Certificate Thumbprint value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificateKeyLength": 4,
    "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
    "certificateValidityPeriod": 9,
    "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
    "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
    "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
    "certificateErrorCode": 4
  }
}
```




