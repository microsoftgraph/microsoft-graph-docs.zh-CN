---
title: 列出 deviceConfigurationUserStatuses
description: 列出 deviceConfigurationUserStatus 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e69ce1d68d675db4a010a3d6ef17c857d7ffeb80
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137474"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="703e7-103">列出 deviceConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="703e7-103">List deviceConfigurationUserStatuses</span></span>

<span data-ttu-id="703e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="703e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="703e7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="703e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="703e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="703e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="703e7-107">列出 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="703e7-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="703e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="703e7-108">Prerequisites</span></span>
<span data-ttu-id="703e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="703e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="703e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="703e7-111">Permission type</span></span>|<span data-ttu-id="703e7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="703e7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="703e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="703e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="703e7-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703e7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="703e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="703e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="703e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="703e7-116">Not supported.</span></span>|
|<span data-ttu-id="703e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="703e7-117">Application</span></span>|<span data-ttu-id="703e7-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703e7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="703e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="703e7-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="703e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="703e7-120">Request headers</span></span>
|<span data-ttu-id="703e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="703e7-121">Header</span></span>|<span data-ttu-id="703e7-122">值</span><span class="sxs-lookup"><span data-stu-id="703e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="703e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="703e7-123">Authorization</span></span>|<span data-ttu-id="703e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="703e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="703e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="703e7-125">Accept</span></span>|<span data-ttu-id="703e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="703e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="703e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="703e7-127">Request body</span></span>
<span data-ttu-id="703e7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="703e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="703e7-129">响应</span><span class="sxs-lookup"><span data-stu-id="703e7-129">Response</span></span>
<span data-ttu-id="703e7-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="703e7-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="703e7-131">示例</span><span class="sxs-lookup"><span data-stu-id="703e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="703e7-132">请求</span><span class="sxs-lookup"><span data-stu-id="703e7-132">Request</span></span>
<span data-ttu-id="703e7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="703e7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="703e7-134">响应</span><span class="sxs-lookup"><span data-stu-id="703e7-134">Response</span></span>
<span data-ttu-id="703e7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="703e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




