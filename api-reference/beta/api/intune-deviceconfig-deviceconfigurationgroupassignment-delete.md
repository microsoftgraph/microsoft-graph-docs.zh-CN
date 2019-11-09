---
title: 删除 deviceConfigurationGroupAssignment
description: 删除 deviceConfigurationGroupAssignment。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7cb59dd04db792bb75a4dbfb228ef4682c22f81
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084466"
---
# <a name="delete-deviceconfigurationgroupassignment"></a><span data-ttu-id="1bea9-103">删除 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1bea9-103">Delete deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="1bea9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1bea9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bea9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1bea9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bea9-106">删除[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1bea9-106">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bea9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bea9-107">Prerequisites</span></span>
<span data-ttu-id="1bea9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bea9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bea9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bea9-110">Permission type</span></span>|<span data-ttu-id="1bea9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bea9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bea9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bea9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bea9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bea9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1bea9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bea9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bea9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bea9-115">Not supported.</span></span>|
|<span data-ttu-id="1bea9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bea9-116">Application</span></span>|<span data-ttu-id="1bea9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bea9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bea9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bea9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1bea9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bea9-119">Request headers</span></span>
|<span data-ttu-id="1bea9-120">标头</span><span class="sxs-lookup"><span data-stu-id="1bea9-120">Header</span></span>|<span data-ttu-id="1bea9-121">值</span><span class="sxs-lookup"><span data-stu-id="1bea9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bea9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bea9-122">Authorization</span></span>|<span data-ttu-id="1bea9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bea9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bea9-124">接受</span><span class="sxs-lookup"><span data-stu-id="1bea9-124">Accept</span></span>|<span data-ttu-id="1bea9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bea9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bea9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bea9-126">Request body</span></span>
<span data-ttu-id="1bea9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bea9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bea9-128">响应</span><span class="sxs-lookup"><span data-stu-id="1bea9-128">Response</span></span>
<span data-ttu-id="1bea9-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1bea9-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bea9-130">示例</span><span class="sxs-lookup"><span data-stu-id="1bea9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bea9-131">请求</span><span class="sxs-lookup"><span data-stu-id="1bea9-131">Request</span></span>
<span data-ttu-id="1bea9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bea9-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="1bea9-133">响应</span><span class="sxs-lookup"><span data-stu-id="1bea9-133">Response</span></span>
<span data-ttu-id="1bea9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bea9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






