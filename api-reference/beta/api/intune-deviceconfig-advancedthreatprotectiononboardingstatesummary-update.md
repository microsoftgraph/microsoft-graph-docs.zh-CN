---
title: 更新 advancedThreatProtectionOnboardingStateSummary
description: 更新 advancedThreatProtectionOnboardingStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e980834c33c7fda9f9ad9f1552516d974c0087d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126834"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="3f4f0-103">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3f4f0-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

<span data-ttu-id="3f4f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f4f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f4f0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f4f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f4f0-107">更新 [advancedThreatProtectionOnboardingStateSummary 对象](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f4f0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f4f0-108">Prerequisites</span></span>
<span data-ttu-id="3f4f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f4f0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f4f0-111">Permission type</span></span>|<span data-ttu-id="3f4f0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f4f0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f4f0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f4f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f4f0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f4f0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f4f0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f4f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f4f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-116">Not supported.</span></span>|
|<span data-ttu-id="3f4f0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f4f0-117">Application</span></span>|<span data-ttu-id="3f4f0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f4f0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f4f0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f4f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3f4f0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f4f0-120">Request headers</span></span>
|<span data-ttu-id="3f4f0-121">标头</span><span class="sxs-lookup"><span data-stu-id="3f4f0-121">Header</span></span>|<span data-ttu-id="3f4f0-122">值</span><span class="sxs-lookup"><span data-stu-id="3f4f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f4f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f4f0-123">Authorization</span></span>|<span data-ttu-id="3f4f0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f4f0-125">接受</span><span class="sxs-lookup"><span data-stu-id="3f4f0-125">Accept</span></span>|<span data-ttu-id="3f4f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f4f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f4f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f4f0-127">Request body</span></span>
<span data-ttu-id="3f4f0-128">在请求正文中，提供 [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="3f4f0-129">下表显示创建 [advancedThreatProtectionOnboardingStateSummary 时所需的属性](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="3f4f0-130">属性</span><span class="sxs-lookup"><span data-stu-id="3f4f0-130">Property</span></span>|<span data-ttu-id="3f4f0-131">类型</span><span class="sxs-lookup"><span data-stu-id="3f4f0-131">Type</span></span>|<span data-ttu-id="3f4f0-132">说明</span><span class="sxs-lookup"><span data-stu-id="3f4f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4f0-133">id</span><span class="sxs-lookup"><span data-stu-id="3f4f0-133">id</span></span>|<span data-ttu-id="3f4f0-134">String</span><span class="sxs-lookup"><span data-stu-id="3f4f0-134">String</span></span>|<span data-ttu-id="3f4f0-135">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3f4f0-135">Unique Identifier</span></span>|
|<span data-ttu-id="3f4f0-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-136">unknownDeviceCount</span></span>|<span data-ttu-id="3f4f0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-137">Int32</span></span>|<span data-ttu-id="3f4f0-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-138">Number of unknown devices</span></span>|
|<span data-ttu-id="3f4f0-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="3f4f0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-140">Int32</span></span>|<span data-ttu-id="3f4f0-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="3f4f0-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-142">compliantDeviceCount</span></span>|<span data-ttu-id="3f4f0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-143">Int32</span></span>|<span data-ttu-id="3f4f0-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-144">Number of compliant devices</span></span>|
|<span data-ttu-id="3f4f0-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-145">remediatedDeviceCount</span></span>|<span data-ttu-id="3f4f0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-146">Int32</span></span>|<span data-ttu-id="3f4f0-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-147">Number of remediated devices</span></span>|
|<span data-ttu-id="3f4f0-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3f4f0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-149">Int32</span></span>|<span data-ttu-id="3f4f0-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3f4f0-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-151">errorDeviceCount</span></span>|<span data-ttu-id="3f4f0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-152">Int32</span></span>|<span data-ttu-id="3f4f0-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-153">Number of error devices</span></span>|
|<span data-ttu-id="3f4f0-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-154">conflictDeviceCount</span></span>|<span data-ttu-id="3f4f0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-155">Int32</span></span>|<span data-ttu-id="3f4f0-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-156">Number of conflict devices</span></span>|
|<span data-ttu-id="3f4f0-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f4f0-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="3f4f0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4f0-158">Int32</span></span>|<span data-ttu-id="3f4f0-159">未分配设备的数量</span><span class="sxs-lookup"><span data-stu-id="3f4f0-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="3f4f0-160">响应</span><span class="sxs-lookup"><span data-stu-id="3f4f0-160">Response</span></span>
<span data-ttu-id="3f4f0-161">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f4f0-162">示例</span><span class="sxs-lookup"><span data-stu-id="3f4f0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f4f0-163">请求</span><span class="sxs-lookup"><span data-stu-id="3f4f0-163">Request</span></span>
<span data-ttu-id="3f4f0-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="3f4f0-165">响应</span><span class="sxs-lookup"><span data-stu-id="3f4f0-165">Response</span></span>
<span data-ttu-id="3f4f0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f4f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```




