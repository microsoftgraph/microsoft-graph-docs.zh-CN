---
title: 获取 managedDeviceCertificateState
description: 读取属性和 managedDeviceCertificateState 对象的关系。
author: tfitzmac
ms.openlocfilehash: 54f276e1639dd5514e7a5ee919a4235d344c6dc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315909"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="49c00-103">获取 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="49c00-103">Get managedDeviceCertificateState</span></span>

> <span data-ttu-id="49c00-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49c00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49c00-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49c00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49c00-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49c00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49c00-107">读取属性和[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="49c00-107">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49c00-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="49c00-108">Prerequisites</span></span>
<span data-ttu-id="49c00-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="49c00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49c00-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="49c00-111">Permission type</span></span>|<span data-ttu-id="49c00-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="49c00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49c00-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49c00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49c00-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49c00-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="49c00-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49c00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49c00-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49c00-116">Not supported.</span></span>|
|<span data-ttu-id="49c00-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="49c00-117">Application</span></span>|<span data-ttu-id="49c00-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="49c00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49c00-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49c00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49c00-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49c00-120">Optional query parameters</span></span>
<span data-ttu-id="49c00-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="49c00-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="49c00-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="49c00-122">Request headers</span></span>
|<span data-ttu-id="49c00-123">标头</span><span class="sxs-lookup"><span data-stu-id="49c00-123">Header</span></span>|<span data-ttu-id="49c00-124">值</span><span class="sxs-lookup"><span data-stu-id="49c00-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49c00-125">授权</span><span class="sxs-lookup"><span data-stu-id="49c00-125">Authorization</span></span>|<span data-ttu-id="49c00-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49c00-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49c00-127">Accept</span><span class="sxs-lookup"><span data-stu-id="49c00-127">Accept</span></span>|<span data-ttu-id="49c00-128">application/json</span><span class="sxs-lookup"><span data-stu-id="49c00-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c00-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="49c00-129">Request body</span></span>
<span data-ttu-id="49c00-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49c00-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49c00-131">响应</span><span class="sxs-lookup"><span data-stu-id="49c00-131">Response</span></span>
<span data-ttu-id="49c00-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49c00-132">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c00-133">示例</span><span class="sxs-lookup"><span data-stu-id="49c00-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="49c00-134">请求</span><span class="sxs-lookup"><span data-stu-id="49c00-134">Request</span></span>
<span data-ttu-id="49c00-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49c00-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="49c00-136">响应</span><span class="sxs-lookup"><span data-stu-id="49c00-136">Response</span></span>
<span data-ttu-id="49c00-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49c00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





