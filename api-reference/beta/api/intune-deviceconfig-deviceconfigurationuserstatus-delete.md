---
title: 删除 deviceConfigurationUserStatus
description: 删除 deviceConfigurationUserStatus。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d8b73b0763822a2a4e22315febc34000225f1db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792861"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="fa158-103">删除 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="fa158-103">Delete deviceConfigurationUserStatus</span></span>

<span data-ttu-id="fa158-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa158-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa158-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa158-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa158-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa158-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa158-107">删除 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="fa158-107">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa158-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa158-108">Prerequisites</span></span>
<span data-ttu-id="fa158-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fa158-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fa158-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa158-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa158-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa158-111">Permission type</span></span>|<span data-ttu-id="fa158-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa158-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa158-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa158-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa158-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa158-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa158-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa158-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa158-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa158-116">Not supported.</span></span>|
|<span data-ttu-id="fa158-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa158-117">Application</span></span>|<span data-ttu-id="fa158-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa158-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa158-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa158-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="fa158-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa158-120">Request headers</span></span>
|<span data-ttu-id="fa158-121">标头</span><span class="sxs-lookup"><span data-stu-id="fa158-121">Header</span></span>|<span data-ttu-id="fa158-122">值</span><span class="sxs-lookup"><span data-stu-id="fa158-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa158-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa158-123">Authorization</span></span>|<span data-ttu-id="fa158-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa158-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa158-125">接受</span><span class="sxs-lookup"><span data-stu-id="fa158-125">Accept</span></span>|<span data-ttu-id="fa158-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa158-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa158-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa158-127">Request body</span></span>
<span data-ttu-id="fa158-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa158-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa158-129">响应</span><span class="sxs-lookup"><span data-stu-id="fa158-129">Response</span></span>
<span data-ttu-id="fa158-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fa158-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fa158-131">示例</span><span class="sxs-lookup"><span data-stu-id="fa158-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa158-132">请求</span><span class="sxs-lookup"><span data-stu-id="fa158-132">Request</span></span>
<span data-ttu-id="fa158-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa158-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="fa158-134">响应</span><span class="sxs-lookup"><span data-stu-id="fa158-134">Response</span></span>
<span data-ttu-id="fa158-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="fa158-135">Here is an example of the response.</span></span> <span data-ttu-id="fa158-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="fa158-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fa158-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fa158-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



