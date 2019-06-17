---
title: 列出 windows81TrustedRootCertificates
description: 列出 windows81TrustedRootCertificate 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcf4b9bd8f83077c871236bdeec686a3e4649a6f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977707"
---
# <a name="list-windows81trustedrootcertificates"></a><span data-ttu-id="ea8d7-103">列出 windows81TrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="ea8d7-103">List windows81TrustedRootCertificates</span></span>

> <span data-ttu-id="ea8d7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea8d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea8d7-106">列出[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-106">List properties and relationships of the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea8d7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea8d7-107">Prerequisites</span></span>
<span data-ttu-id="ea8d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea8d7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea8d7-110">Permission type</span></span>|<span data-ttu-id="ea8d7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea8d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea8d7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea8d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea8d7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea8d7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea8d7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea8d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea8d7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-115">Not supported.</span></span>|
|<span data-ttu-id="ea8d7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea8d7-116">Application</span></span>|<span data-ttu-id="ea8d7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea8d7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea8d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="ea8d7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea8d7-119">Request headers</span></span>
|<span data-ttu-id="ea8d7-120">标头</span><span class="sxs-lookup"><span data-stu-id="ea8d7-120">Header</span></span>|<span data-ttu-id="ea8d7-121">值</span><span class="sxs-lookup"><span data-stu-id="ea8d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea8d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea8d7-122">Authorization</span></span>|<span data-ttu-id="ea8d7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea8d7-124">接受</span><span class="sxs-lookup"><span data-stu-id="ea8d7-124">Accept</span></span>|<span data-ttu-id="ea8d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea8d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea8d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea8d7-126">Request body</span></span>
<span data-ttu-id="ea8d7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea8d7-128">响应</span><span class="sxs-lookup"><span data-stu-id="ea8d7-128">Response</span></span>
<span data-ttu-id="ea8d7-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-129">If successful, this method returns a `200 OK` response code and a collection of [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea8d7-130">示例</span><span class="sxs-lookup"><span data-stu-id="ea8d7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea8d7-131">请求</span><span class="sxs-lookup"><span data-stu-id="ea8d7-131">Request</span></span>
<span data-ttu-id="ea8d7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

### <a name="response"></a><span data-ttu-id="ea8d7-133">响应</span><span class="sxs-lookup"><span data-stu-id="ea8d7-133">Response</span></span>
<span data-ttu-id="ea8d7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea8d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1543

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
      "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value",
      "destinationStore": "computerCertStoreIntermediate"
    }
  ]
}
```





