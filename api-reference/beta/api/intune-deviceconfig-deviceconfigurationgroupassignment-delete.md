---
title: 删除 deviceConfigurationGroupAssignment
description: 删除 deviceConfigurationGroupAssignment。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32e1152ef924fe6be5dc2df136eccbb2ec6398de
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792910"
---
# <a name="delete-deviceconfigurationgroupassignment"></a><span data-ttu-id="c1021-103">删除 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="c1021-103">Delete deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="c1021-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1021-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1021-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1021-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1021-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1021-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1021-107">删除[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c1021-107">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1021-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1021-108">Prerequisites</span></span>
<span data-ttu-id="c1021-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c1021-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c1021-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1021-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1021-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1021-111">Permission type</span></span>|<span data-ttu-id="c1021-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1021-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1021-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1021-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1021-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1021-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1021-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1021-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1021-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1021-116">Not supported.</span></span>|
|<span data-ttu-id="c1021-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1021-117">Application</span></span>|<span data-ttu-id="c1021-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1021-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1021-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1021-119">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1021-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1021-120">Request headers</span></span>
|<span data-ttu-id="c1021-121">标头</span><span class="sxs-lookup"><span data-stu-id="c1021-121">Header</span></span>|<span data-ttu-id="c1021-122">值</span><span class="sxs-lookup"><span data-stu-id="c1021-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1021-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1021-123">Authorization</span></span>|<span data-ttu-id="c1021-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1021-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1021-125">接受</span><span class="sxs-lookup"><span data-stu-id="c1021-125">Accept</span></span>|<span data-ttu-id="c1021-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1021-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1021-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1021-127">Request body</span></span>
<span data-ttu-id="c1021-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1021-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1021-129">响应</span><span class="sxs-lookup"><span data-stu-id="c1021-129">Response</span></span>
<span data-ttu-id="c1021-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c1021-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c1021-131">示例</span><span class="sxs-lookup"><span data-stu-id="c1021-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1021-132">请求</span><span class="sxs-lookup"><span data-stu-id="c1021-132">Request</span></span>
<span data-ttu-id="c1021-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1021-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c1021-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1021-134">Response</span></span>
<span data-ttu-id="c1021-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c1021-135">Here is an example of the response.</span></span> <span data-ttu-id="c1021-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c1021-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c1021-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c1021-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



