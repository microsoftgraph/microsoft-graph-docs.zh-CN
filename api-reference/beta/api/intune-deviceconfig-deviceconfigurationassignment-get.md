---
title: 获取 deviceConfigurationAssignment
description: 读取 deviceConfigurationAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1841df035409752dea3d8ce5ce7375074354240e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171622"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="d652a-103">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d652a-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="d652a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d652a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d652a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d652a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d652a-106">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d652a-106">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d652a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d652a-107">Prerequisites</span></span>
<span data-ttu-id="d652a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d652a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d652a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d652a-110">Permission type</span></span>|<span data-ttu-id="d652a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d652a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d652a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d652a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d652a-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d652a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d652a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d652a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d652a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d652a-115">Not supported.</span></span>|
|<span data-ttu-id="d652a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d652a-116">Application</span></span>|<span data-ttu-id="d652a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d652a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d652a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d652a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d652a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d652a-119">Optional query parameters</span></span>
<span data-ttu-id="d652a-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d652a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d652a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d652a-121">Request headers</span></span>
|<span data-ttu-id="d652a-122">标头</span><span class="sxs-lookup"><span data-stu-id="d652a-122">Header</span></span>|<span data-ttu-id="d652a-123">值</span><span class="sxs-lookup"><span data-stu-id="d652a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d652a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d652a-124">Authorization</span></span>|<span data-ttu-id="d652a-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d652a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d652a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d652a-126">Accept</span></span>|<span data-ttu-id="d652a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d652a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d652a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d652a-128">Request body</span></span>
<span data-ttu-id="d652a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d652a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d652a-130">响应</span><span class="sxs-lookup"><span data-stu-id="d652a-130">Response</span></span>
<span data-ttu-id="d652a-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d652a-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d652a-132">示例</span><span class="sxs-lookup"><span data-stu-id="d652a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d652a-133">请求</span><span class="sxs-lookup"><span data-stu-id="d652a-133">Request</span></span>
<span data-ttu-id="d652a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d652a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d652a-135">响应</span><span class="sxs-lookup"><span data-stu-id="d652a-135">Response</span></span>
<span data-ttu-id="d652a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d652a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




