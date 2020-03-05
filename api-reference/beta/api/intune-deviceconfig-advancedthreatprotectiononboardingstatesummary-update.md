---
title: 更新 advancedThreatProtectionOnboardingStateSummary
description: 更新 advancedThreatProtectionOnboardingStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 002ba03a5ea0681b1c88598f9e6f20885ad8b762
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450144"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="03771-103">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="03771-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

<span data-ttu-id="03771-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="03771-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03771-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03771-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03771-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03771-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03771-107">更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03771-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03771-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03771-108">Prerequisites</span></span>
<span data-ttu-id="03771-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03771-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03771-111">Permission type</span></span>|<span data-ttu-id="03771-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03771-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03771-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03771-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03771-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03771-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03771-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03771-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03771-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03771-116">Not supported.</span></span>|
|<span data-ttu-id="03771-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03771-117">Application</span></span>|<span data-ttu-id="03771-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03771-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03771-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03771-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="03771-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03771-120">Request headers</span></span>
|<span data-ttu-id="03771-121">标头</span><span class="sxs-lookup"><span data-stu-id="03771-121">Header</span></span>|<span data-ttu-id="03771-122">值</span><span class="sxs-lookup"><span data-stu-id="03771-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03771-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03771-123">Authorization</span></span>|<span data-ttu-id="03771-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03771-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03771-125">接受</span><span class="sxs-lookup"><span data-stu-id="03771-125">Accept</span></span>|<span data-ttu-id="03771-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03771-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03771-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03771-127">Request body</span></span>
<span data-ttu-id="03771-128">在请求正文中，提供[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03771-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="03771-129">下表显示创建[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03771-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="03771-130">属性</span><span class="sxs-lookup"><span data-stu-id="03771-130">Property</span></span>|<span data-ttu-id="03771-131">类型</span><span class="sxs-lookup"><span data-stu-id="03771-131">Type</span></span>|<span data-ttu-id="03771-132">说明</span><span class="sxs-lookup"><span data-stu-id="03771-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03771-133">id</span><span class="sxs-lookup"><span data-stu-id="03771-133">id</span></span>|<span data-ttu-id="03771-134">String</span><span class="sxs-lookup"><span data-stu-id="03771-134">String</span></span>|<span data-ttu-id="03771-135">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="03771-135">Unique Identifier</span></span>|
|<span data-ttu-id="03771-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-136">unknownDeviceCount</span></span>|<span data-ttu-id="03771-137">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-137">Int32</span></span>|<span data-ttu-id="03771-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-138">Number of unknown devices</span></span>|
|<span data-ttu-id="03771-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="03771-140">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-140">Int32</span></span>|<span data-ttu-id="03771-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="03771-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-142">compliantDeviceCount</span></span>|<span data-ttu-id="03771-143">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-143">Int32</span></span>|<span data-ttu-id="03771-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-144">Number of compliant devices</span></span>|
|<span data-ttu-id="03771-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-145">remediatedDeviceCount</span></span>|<span data-ttu-id="03771-146">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-146">Int32</span></span>|<span data-ttu-id="03771-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-147">Number of remediated devices</span></span>|
|<span data-ttu-id="03771-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="03771-149">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-149">Int32</span></span>|<span data-ttu-id="03771-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="03771-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-151">errorDeviceCount</span></span>|<span data-ttu-id="03771-152">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-152">Int32</span></span>|<span data-ttu-id="03771-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-153">Number of error devices</span></span>|
|<span data-ttu-id="03771-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-154">conflictDeviceCount</span></span>|<span data-ttu-id="03771-155">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-155">Int32</span></span>|<span data-ttu-id="03771-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-156">Number of conflict devices</span></span>|
|<span data-ttu-id="03771-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03771-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="03771-158">Int32</span><span class="sxs-lookup"><span data-stu-id="03771-158">Int32</span></span>|<span data-ttu-id="03771-159">未分配设备的数量</span><span class="sxs-lookup"><span data-stu-id="03771-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="03771-160">响应</span><span class="sxs-lookup"><span data-stu-id="03771-160">Response</span></span>
<span data-ttu-id="03771-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="03771-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03771-162">示例</span><span class="sxs-lookup"><span data-stu-id="03771-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="03771-163">请求</span><span class="sxs-lookup"><span data-stu-id="03771-163">Request</span></span>
<span data-ttu-id="03771-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03771-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03771-165">响应</span><span class="sxs-lookup"><span data-stu-id="03771-165">Response</span></span>
<span data-ttu-id="03771-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03771-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





