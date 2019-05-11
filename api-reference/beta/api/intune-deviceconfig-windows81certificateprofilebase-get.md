---
title: 获取 windows81CertificateProfileBase
description: 读取 windows81CertificateProfileBase 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540e526324fbe9f1a54c2a319510508943ee90b1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918351"
---
# <a name="get-windows81certificateprofilebase"></a><span data-ttu-id="d494e-103">获取 windows81CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="d494e-103">Get windows81CertificateProfileBase</span></span>

> <span data-ttu-id="d494e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d494e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d494e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d494e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d494e-106">读取[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d494e-106">Read properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d494e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d494e-107">Prerequisites</span></span>
<span data-ttu-id="d494e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d494e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d494e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d494e-110">Permission type</span></span>|<span data-ttu-id="d494e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d494e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d494e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d494e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d494e-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d494e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d494e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d494e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d494e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d494e-115">Not supported.</span></span>|
|<span data-ttu-id="d494e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d494e-116">Application</span></span>|<span data-ttu-id="d494e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d494e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d494e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d494e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d494e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d494e-119">Optional query parameters</span></span>
<span data-ttu-id="d494e-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d494e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d494e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d494e-121">Request headers</span></span>
|<span data-ttu-id="d494e-122">标头</span><span class="sxs-lookup"><span data-stu-id="d494e-122">Header</span></span>|<span data-ttu-id="d494e-123">值</span><span class="sxs-lookup"><span data-stu-id="d494e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d494e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d494e-124">Authorization</span></span>|<span data-ttu-id="d494e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d494e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d494e-126">接受</span><span class="sxs-lookup"><span data-stu-id="d494e-126">Accept</span></span>|<span data-ttu-id="d494e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d494e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d494e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d494e-128">Request body</span></span>
<span data-ttu-id="d494e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d494e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d494e-130">响应</span><span class="sxs-lookup"><span data-stu-id="d494e-130">Response</span></span>
<span data-ttu-id="d494e-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d494e-131">If successful, this method returns a `200 OK` response code and [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d494e-132">示例</span><span class="sxs-lookup"><span data-stu-id="d494e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d494e-133">请求</span><span class="sxs-lookup"><span data-stu-id="d494e-133">Request</span></span>
<span data-ttu-id="d494e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d494e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d494e-135">响应</span><span class="sxs-lookup"><span data-stu-id="d494e-135">Response</span></span>
<span data-ttu-id="d494e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d494e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1167

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
    "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "customSubjectAlternativeNames": [
      {
        "@odata.type": "microsoft.graph.customSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ]
  }
}
```




