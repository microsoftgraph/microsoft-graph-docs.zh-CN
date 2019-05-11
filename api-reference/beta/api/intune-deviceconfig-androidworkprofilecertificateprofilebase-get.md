---
title: 获取 androidWorkProfileCertificateProfileBase
description: 读取 androidWorkProfileCertificateProfileBase 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c606d13eeb267f6e8275b62b4e2ed4f3eb5551e0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928678"
---
# <a name="get-androidworkprofilecertificateprofilebase"></a><span data-ttu-id="1c9ac-103">获取 androidWorkProfileCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="1c9ac-103">Get androidWorkProfileCertificateProfileBase</span></span>

> <span data-ttu-id="1c9ac-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c9ac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c9ac-106">读取[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-106">Read properties and relationships of the [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c9ac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c9ac-107">Prerequisites</span></span>
<span data-ttu-id="1c9ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c9ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c9ac-110">Permission type</span></span>|<span data-ttu-id="1c9ac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1c9ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c9ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c9ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c9ac-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c9ac-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c9ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c9ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c9ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-115">Not supported.</span></span>|
|<span data-ttu-id="1c9ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c9ac-116">Application</span></span>|<span data-ttu-id="1c9ac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c9ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c9ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEasEmailProfileBase/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c9ac-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1c9ac-119">Optional query parameters</span></span>
<span data-ttu-id="1c9ac-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c9ac-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c9ac-121">Request headers</span></span>
|<span data-ttu-id="1c9ac-122">标头</span><span class="sxs-lookup"><span data-stu-id="1c9ac-122">Header</span></span>|<span data-ttu-id="1c9ac-123">值</span><span class="sxs-lookup"><span data-stu-id="1c9ac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c9ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c9ac-124">Authorization</span></span>|<span data-ttu-id="1c9ac-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c9ac-126">接受</span><span class="sxs-lookup"><span data-stu-id="1c9ac-126">Accept</span></span>|<span data-ttu-id="1c9ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1c9ac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c9ac-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c9ac-128">Request body</span></span>
<span data-ttu-id="1c9ac-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c9ac-130">响应</span><span class="sxs-lookup"><span data-stu-id="1c9ac-130">Response</span></span>
<span data-ttu-id="1c9ac-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c9ac-132">示例</span><span class="sxs-lookup"><span data-stu-id="1c9ac-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c9ac-133">请求</span><span class="sxs-lookup"><span data-stu-id="1c9ac-133">Request</span></span>
<span data-ttu-id="1c9ac-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
```

### <a name="response"></a><span data-ttu-id="1c9ac-135">响应</span><span class="sxs-lookup"><span data-stu-id="1c9ac-135">Response</span></span>
<span data-ttu-id="1c9ac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c9ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 919

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCertificateProfileBase",
    "id": "4a559c8b-9c8b-4a55-8b9c-554a8b9c554a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "subjectAlternativeNameType": "emailAddress"
  }
}
```




