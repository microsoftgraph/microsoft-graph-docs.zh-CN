---
title: 列出 androidDeviceOwnerPkcsCertificateProfiles
description: 列出 androidDeviceOwnerPkcsCertificateProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb0395da82f32b016222b12797da7ccb90fc6e8c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793085"
---
# <a name="list-androiddeviceownerpkcscertificateprofiles"></a><span data-ttu-id="3d5d9-103">列出 androidDeviceOwnerPkcsCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="3d5d9-103">List androidDeviceOwnerPkcsCertificateProfiles</span></span>

<span data-ttu-id="3d5d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d5d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d5d9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d5d9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d5d9-107">列出[androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-107">List properties and relationships of the [androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d5d9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d5d9-108">Prerequisites</span></span>
<span data-ttu-id="3d5d9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3d5d9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3d5d9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d5d9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d5d9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d5d9-111">Permission type</span></span>|<span data-ttu-id="3d5d9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d5d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d5d9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d5d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d5d9-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d5d9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3d5d9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d5d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d5d9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-116">Not supported.</span></span>|
|<span data-ttu-id="3d5d9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d5d9-117">Application</span></span>|<span data-ttu-id="3d5d9-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d5d9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d5d9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d5d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d5d9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d5d9-120">Request headers</span></span>
|<span data-ttu-id="3d5d9-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d5d9-121">Header</span></span>|<span data-ttu-id="3d5d9-122">值</span><span class="sxs-lookup"><span data-stu-id="3d5d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d5d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d5d9-123">Authorization</span></span>|<span data-ttu-id="3d5d9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d5d9-125">接受</span><span class="sxs-lookup"><span data-stu-id="3d5d9-125">Accept</span></span>|<span data-ttu-id="3d5d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d5d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d5d9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d5d9-127">Request body</span></span>
<span data-ttu-id="3d5d9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d5d9-129">响应</span><span class="sxs-lookup"><span data-stu-id="3d5d9-129">Response</span></span>
<span data-ttu-id="3d5d9-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d5d9-131">示例</span><span class="sxs-lookup"><span data-stu-id="3d5d9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d5d9-132">请求</span><span class="sxs-lookup"><span data-stu-id="3d5d9-132">Request</span></span>
<span data-ttu-id="3d5d9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d5d9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3d5d9-134">响应</span><span class="sxs-lookup"><span data-stu-id="3d5d9-134">Response</span></span>
<span data-ttu-id="3d5d9-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3d5d9-135">Here is an example of the response.</span></span> <span data-ttu-id="3d5d9-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3d5d9-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3d5d9-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3d5d9-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2515

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerPkcsCertificateProfile",
      "id": "5e86a0e6-a0e6-5e86-e6a0-865ee6a0865e",
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
      "subjectNameFormat": "commonNameIncludingEmail",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameType": "emailAddress",
      "certificationAuthority": "Certification Authority value",
      "certificationAuthorityName": "Certification Authority Name value",
      "certificationAuthorityType": "microsoft",
      "certificateTemplateName": "Certificate Template Name value",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "subjectNameFormatString": "Subject Name Format String value",
      "certificateStore": "machine",
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```



