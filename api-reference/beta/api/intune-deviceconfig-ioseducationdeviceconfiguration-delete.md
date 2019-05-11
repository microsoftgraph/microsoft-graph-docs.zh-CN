---
title: 删除 iosEducationDeviceConfiguration
description: 删除 iosEducationDeviceConfiguration。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53cb3f564f8ef681b0a686744b9929141f20ea6e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923557"
---
# <a name="delete-ioseducationdeviceconfiguration"></a><span data-ttu-id="6aaeb-103">删除 iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aaeb-103">Delete iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="6aaeb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aaeb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aaeb-106">删除[iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-106">Deletes a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aaeb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6aaeb-107">Prerequisites</span></span>
<span data-ttu-id="6aaeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aaeb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6aaeb-110">Permission type</span></span>|<span data-ttu-id="6aaeb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6aaeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aaeb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6aaeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aaeb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aaeb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aaeb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6aaeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aaeb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-115">Not supported.</span></span>|
|<span data-ttu-id="6aaeb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6aaeb-116">Application</span></span>|<span data-ttu-id="6aaeb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aaeb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6aaeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6aaeb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6aaeb-119">Request headers</span></span>
|<span data-ttu-id="6aaeb-120">标头</span><span class="sxs-lookup"><span data-stu-id="6aaeb-120">Header</span></span>|<span data-ttu-id="6aaeb-121">值</span><span class="sxs-lookup"><span data-stu-id="6aaeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aaeb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aaeb-122">Authorization</span></span>|<span data-ttu-id="6aaeb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aaeb-124">接受</span><span class="sxs-lookup"><span data-stu-id="6aaeb-124">Accept</span></span>|<span data-ttu-id="6aaeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aaeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aaeb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6aaeb-126">Request body</span></span>
<span data-ttu-id="6aaeb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aaeb-128">响应</span><span class="sxs-lookup"><span data-stu-id="6aaeb-128">Response</span></span>
<span data-ttu-id="6aaeb-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6aaeb-130">示例</span><span class="sxs-lookup"><span data-stu-id="6aaeb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aaeb-131">请求</span><span class="sxs-lookup"><span data-stu-id="6aaeb-131">Request</span></span>
<span data-ttu-id="6aaeb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6aaeb-133">响应</span><span class="sxs-lookup"><span data-stu-id="6aaeb-133">Response</span></span>
<span data-ttu-id="6aaeb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6aaeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




