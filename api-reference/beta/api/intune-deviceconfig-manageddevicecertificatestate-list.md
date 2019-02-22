---
title: 列出 managedDeviceCertificateStates
description: 列出 managedDeviceCertificateState 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3497a3641ff9823e94bd2bfb3ca77d99a4ef344
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146492"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="91689-103">列出 managedDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="91689-103">List managedDeviceCertificateStates</span></span>

> <span data-ttu-id="91689-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91689-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91689-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91689-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91689-106">列出[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91689-106">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91689-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="91689-107">Prerequisites</span></span>
<span data-ttu-id="91689-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="91689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="91689-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="91689-110">Permission type</span></span>|<span data-ttu-id="91689-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91689-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91689-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91689-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91689-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="91689-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="91689-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91689-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91689-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="91689-115">Not supported.</span></span>|
|<span data-ttu-id="91689-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="91689-116">Application</span></span>|<span data-ttu-id="91689-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="91689-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91689-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91689-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="91689-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="91689-119">Request headers</span></span>
|<span data-ttu-id="91689-120">标头</span><span class="sxs-lookup"><span data-stu-id="91689-120">Header</span></span>|<span data-ttu-id="91689-121">值</span><span class="sxs-lookup"><span data-stu-id="91689-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91689-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91689-122">Authorization</span></span>|<span data-ttu-id="91689-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91689-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91689-124">Accept</span><span class="sxs-lookup"><span data-stu-id="91689-124">Accept</span></span>|<span data-ttu-id="91689-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91689-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91689-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91689-126">Request body</span></span>
<span data-ttu-id="91689-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91689-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91689-128">响应</span><span class="sxs-lookup"><span data-stu-id="91689-128">Response</span></span>
<span data-ttu-id="91689-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="91689-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91689-130">示例</span><span class="sxs-lookup"><span data-stu-id="91689-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="91689-131">请求</span><span class="sxs-lookup"><span data-stu-id="91689-131">Request</span></span>
<span data-ttu-id="91689-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91689-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="91689-133">响应</span><span class="sxs-lookup"><span data-stu-id="91689-133">Response</span></span>
<span data-ttu-id="91689-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91689-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1703

{
  "value": [
    {
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
  ]
}
```




