---
title: 删除 advancedThreatProtectionOnboardingDeviceSettingState
description: 删除 advancedThreatProtectionOnboardingDeviceSettingState。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e1ea0efa00feb2de2f80a167f494227fd92ece9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982495"
---
# <a name="delete-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="2a410-103">删除 advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="2a410-103">Delete advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="2a410-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a410-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a410-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a410-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a410-106">删除[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="2a410-106">Deletes a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a410-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a410-107">Prerequisites</span></span>
<span data-ttu-id="2a410-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a410-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a410-110">Permission type</span></span>|<span data-ttu-id="2a410-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a410-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a410-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a410-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a410-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a410-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a410-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a410-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a410-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a410-115">Not supported.</span></span>|
|<span data-ttu-id="2a410-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a410-116">Application</span></span>|<span data-ttu-id="2a410-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a410-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a410-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a410-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2a410-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a410-119">Request headers</span></span>
|<span data-ttu-id="2a410-120">标头</span><span class="sxs-lookup"><span data-stu-id="2a410-120">Header</span></span>|<span data-ttu-id="2a410-121">值</span><span class="sxs-lookup"><span data-stu-id="2a410-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a410-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a410-122">Authorization</span></span>|<span data-ttu-id="2a410-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a410-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a410-124">接受</span><span class="sxs-lookup"><span data-stu-id="2a410-124">Accept</span></span>|<span data-ttu-id="2a410-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a410-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a410-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a410-126">Request body</span></span>
<span data-ttu-id="2a410-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a410-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a410-128">响应</span><span class="sxs-lookup"><span data-stu-id="2a410-128">Response</span></span>
<span data-ttu-id="2a410-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2a410-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a410-130">示例</span><span class="sxs-lookup"><span data-stu-id="2a410-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a410-131">请求</span><span class="sxs-lookup"><span data-stu-id="2a410-131">Request</span></span>
<span data-ttu-id="2a410-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a410-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="2a410-133">响应</span><span class="sxs-lookup"><span data-stu-id="2a410-133">Response</span></span>
<span data-ttu-id="2a410-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a410-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




