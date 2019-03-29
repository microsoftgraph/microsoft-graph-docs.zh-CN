---
title: 列出 deviceConfigurationAssignments
description: 列出 deviceConfigurationAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b39206581090300fdf8769ef972b3b968b10faaa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984946"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="8cf88-103">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="8cf88-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="8cf88-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8cf88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cf88-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8cf88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cf88-106">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8cf88-106">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cf88-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8cf88-107">Prerequisites</span></span>
<span data-ttu-id="8cf88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cf88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf88-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cf88-110">Permission type</span></span>|<span data-ttu-id="8cf88-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8cf88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cf88-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cf88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cf88-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cf88-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8cf88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cf88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cf88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cf88-115">Not supported.</span></span>|
|<span data-ttu-id="8cf88-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cf88-116">Application</span></span>|<span data-ttu-id="8cf88-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cf88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cf88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cf88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8cf88-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cf88-119">Request headers</span></span>
|<span data-ttu-id="8cf88-120">标头</span><span class="sxs-lookup"><span data-stu-id="8cf88-120">Header</span></span>|<span data-ttu-id="8cf88-121">值</span><span class="sxs-lookup"><span data-stu-id="8cf88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cf88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cf88-122">Authorization</span></span>|<span data-ttu-id="8cf88-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8cf88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cf88-124">接受</span><span class="sxs-lookup"><span data-stu-id="8cf88-124">Accept</span></span>|<span data-ttu-id="8cf88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cf88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cf88-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cf88-126">Request body</span></span>
<span data-ttu-id="8cf88-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8cf88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cf88-128">响应</span><span class="sxs-lookup"><span data-stu-id="8cf88-128">Response</span></span>
<span data-ttu-id="8cf88-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8cf88-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cf88-130">示例</span><span class="sxs-lookup"><span data-stu-id="8cf88-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cf88-131">请求</span><span class="sxs-lookup"><span data-stu-id="8cf88-131">Request</span></span>
<span data-ttu-id="8cf88-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8cf88-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="8cf88-133">响应</span><span class="sxs-lookup"><span data-stu-id="8cf88-133">Response</span></span>
<span data-ttu-id="8cf88-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8cf88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




