---
title: 列出 deviceConfigurationUserStatuses
description: 列出 deviceConfigurationUserStatus 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 013bbcd80438150e4fe08c61f56b9efd491e2494
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174688"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="13a1e-103">列出 deviceConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="13a1e-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="13a1e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13a1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13a1e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13a1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a1e-106">列出 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13a1e-106">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13a1e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="13a1e-107">Prerequisites</span></span>
<span data-ttu-id="13a1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13a1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a1e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="13a1e-110">Permission type</span></span>|<span data-ttu-id="13a1e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="13a1e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13a1e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13a1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13a1e-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13a1e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13a1e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13a1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13a1e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13a1e-115">Not supported.</span></span>|
|<span data-ttu-id="13a1e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="13a1e-116">Application</span></span>|<span data-ttu-id="13a1e-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13a1e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13a1e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13a1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="13a1e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="13a1e-119">Request headers</span></span>
|<span data-ttu-id="13a1e-120">标头</span><span class="sxs-lookup"><span data-stu-id="13a1e-120">Header</span></span>|<span data-ttu-id="13a1e-121">值</span><span class="sxs-lookup"><span data-stu-id="13a1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13a1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13a1e-122">Authorization</span></span>|<span data-ttu-id="13a1e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13a1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13a1e-124">接受</span><span class="sxs-lookup"><span data-stu-id="13a1e-124">Accept</span></span>|<span data-ttu-id="13a1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13a1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a1e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="13a1e-126">Request body</span></span>
<span data-ttu-id="13a1e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13a1e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13a1e-128">响应</span><span class="sxs-lookup"><span data-stu-id="13a1e-128">Response</span></span>
<span data-ttu-id="13a1e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="13a1e-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a1e-130">示例</span><span class="sxs-lookup"><span data-stu-id="13a1e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13a1e-131">请求</span><span class="sxs-lookup"><span data-stu-id="13a1e-131">Request</span></span>
<span data-ttu-id="13a1e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13a1e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="13a1e-133">响应</span><span class="sxs-lookup"><span data-stu-id="13a1e-133">Response</span></span>
<span data-ttu-id="13a1e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13a1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




