---
title: 删除 advancedThreatProtectionOnboardingDeviceSettingState
description: 删除 advancedThreatProtectionOnboardingDeviceSettingState。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e3ca744a70d271cbd2a5b368022e7311a53cc1f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170334"
---
# <a name="delete-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="95b24-103">删除 advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="95b24-103">Delete advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="95b24-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95b24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95b24-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95b24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b24-106">删除[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="95b24-106">Deletes a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95b24-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95b24-107">Prerequisites</span></span>
<span data-ttu-id="95b24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95b24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95b24-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95b24-110">Permission type</span></span>|<span data-ttu-id="95b24-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95b24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b24-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95b24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95b24-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b24-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95b24-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95b24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b24-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95b24-115">Not supported.</span></span>|
|<span data-ttu-id="95b24-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95b24-116">Application</span></span>|<span data-ttu-id="95b24-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b24-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b24-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95b24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="95b24-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95b24-119">Request headers</span></span>
|<span data-ttu-id="95b24-120">标头</span><span class="sxs-lookup"><span data-stu-id="95b24-120">Header</span></span>|<span data-ttu-id="95b24-121">值</span><span class="sxs-lookup"><span data-stu-id="95b24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95b24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95b24-122">Authorization</span></span>|<span data-ttu-id="95b24-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95b24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95b24-124">接受</span><span class="sxs-lookup"><span data-stu-id="95b24-124">Accept</span></span>|<span data-ttu-id="95b24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95b24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b24-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95b24-126">Request body</span></span>
<span data-ttu-id="95b24-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="95b24-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95b24-128">响应</span><span class="sxs-lookup"><span data-stu-id="95b24-128">Response</span></span>
<span data-ttu-id="95b24-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="95b24-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="95b24-130">示例</span><span class="sxs-lookup"><span data-stu-id="95b24-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95b24-131">请求</span><span class="sxs-lookup"><span data-stu-id="95b24-131">Request</span></span>
<span data-ttu-id="95b24-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95b24-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="95b24-133">响应</span><span class="sxs-lookup"><span data-stu-id="95b24-133">Response</span></span>
<span data-ttu-id="95b24-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95b24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




