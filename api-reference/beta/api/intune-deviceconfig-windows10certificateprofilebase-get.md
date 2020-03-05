---
title: 获取 windows10CertificateProfileBase
description: 读取 windows10CertificateProfileBase 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f20311d3a4a45a52bf4b51b31a12552c827cbda
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42482151"
---
# <a name="get-windows10certificateprofilebase"></a><span data-ttu-id="76562-103">获取 windows10CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="76562-103">Get windows10CertificateProfileBase</span></span>

<span data-ttu-id="76562-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="76562-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76562-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76562-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76562-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76562-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76562-107">读取[windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76562-107">Read properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76562-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="76562-108">Prerequisites</span></span>
<span data-ttu-id="76562-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76562-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76562-111">Permission type</span></span>|<span data-ttu-id="76562-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76562-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76562-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76562-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76562-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76562-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="76562-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76562-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76562-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76562-116">Not supported.</span></span>|
|<span data-ttu-id="76562-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="76562-117">Application</span></span>|<span data-ttu-id="76562-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76562-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76562-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76562-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76562-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76562-120">Optional query parameters</span></span>
<span data-ttu-id="76562-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76562-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76562-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="76562-122">Request headers</span></span>
|<span data-ttu-id="76562-123">标头</span><span class="sxs-lookup"><span data-stu-id="76562-123">Header</span></span>|<span data-ttu-id="76562-124">值</span><span class="sxs-lookup"><span data-stu-id="76562-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76562-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="76562-125">Authorization</span></span>|<span data-ttu-id="76562-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76562-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76562-127">接受</span><span class="sxs-lookup"><span data-stu-id="76562-127">Accept</span></span>|<span data-ttu-id="76562-128">application/json</span><span class="sxs-lookup"><span data-stu-id="76562-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76562-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="76562-129">Request body</span></span>
<span data-ttu-id="76562-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76562-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76562-131">响应</span><span class="sxs-lookup"><span data-stu-id="76562-131">Response</span></span>
<span data-ttu-id="76562-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="76562-132">If successful, this method returns a `200 OK` response code and [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76562-133">示例</span><span class="sxs-lookup"><span data-stu-id="76562-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="76562-134">请求</span><span class="sxs-lookup"><span data-stu-id="76562-134">Request</span></span>
<span data-ttu-id="76562-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76562-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="76562-136">响应</span><span class="sxs-lookup"><span data-stu-id="76562-136">Response</span></span>
<span data-ttu-id="76562-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76562-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1578

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CertificateProfileBase",
    "id": "1f01ffc6-ffc6-1f01-c6ff-011fc6ff011f",
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
    "renewalThresholdPercentage": 10,
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```





