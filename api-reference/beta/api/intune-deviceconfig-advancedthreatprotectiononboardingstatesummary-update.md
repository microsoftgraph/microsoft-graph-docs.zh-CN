---
title: 更新 advancedThreatProtectionOnboardingStateSummary
description: 更新 advancedThreatProtectionOnboardingStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e016ad6a390d09466bf4956c585911669437f82b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958461"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="28e78-103">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="28e78-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="28e78-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28e78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28e78-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28e78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28e78-106">更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28e78-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28e78-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="28e78-107">Prerequisites</span></span>
<span data-ttu-id="28e78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28e78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28e78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28e78-110">Permission type</span></span>|<span data-ttu-id="28e78-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="28e78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28e78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28e78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28e78-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28e78-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28e78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28e78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28e78-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28e78-115">Not supported.</span></span>|
|<span data-ttu-id="28e78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28e78-116">Application</span></span>|<span data-ttu-id="28e78-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="28e78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28e78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28e78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="28e78-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28e78-119">Request headers</span></span>
|<span data-ttu-id="28e78-120">标头</span><span class="sxs-lookup"><span data-stu-id="28e78-120">Header</span></span>|<span data-ttu-id="28e78-121">值</span><span class="sxs-lookup"><span data-stu-id="28e78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28e78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28e78-122">Authorization</span></span>|<span data-ttu-id="28e78-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28e78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28e78-124">接受</span><span class="sxs-lookup"><span data-stu-id="28e78-124">Accept</span></span>|<span data-ttu-id="28e78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28e78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28e78-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28e78-126">Request body</span></span>
<span data-ttu-id="28e78-127">在请求正文中, 提供[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28e78-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="28e78-128">下表显示创建[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28e78-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="28e78-129">属性</span><span class="sxs-lookup"><span data-stu-id="28e78-129">Property</span></span>|<span data-ttu-id="28e78-130">类型</span><span class="sxs-lookup"><span data-stu-id="28e78-130">Type</span></span>|<span data-ttu-id="28e78-131">说明</span><span class="sxs-lookup"><span data-stu-id="28e78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28e78-132">id</span><span class="sxs-lookup"><span data-stu-id="28e78-132">id</span></span>|<span data-ttu-id="28e78-133">String</span><span class="sxs-lookup"><span data-stu-id="28e78-133">String</span></span>|<span data-ttu-id="28e78-134">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="28e78-134">Unique Identifier</span></span>|
|<span data-ttu-id="28e78-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-135">unknownDeviceCount</span></span>|<span data-ttu-id="28e78-136">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-136">Int32</span></span>|<span data-ttu-id="28e78-137">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-137">Number of unknown devices</span></span>|
|<span data-ttu-id="28e78-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="28e78-139">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-139">Int32</span></span>|<span data-ttu-id="28e78-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="28e78-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-141">compliantDeviceCount</span></span>|<span data-ttu-id="28e78-142">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-142">Int32</span></span>|<span data-ttu-id="28e78-143">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-143">Number of compliant devices</span></span>|
|<span data-ttu-id="28e78-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-144">remediatedDeviceCount</span></span>|<span data-ttu-id="28e78-145">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-145">Int32</span></span>|<span data-ttu-id="28e78-146">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-146">Number of remediated devices</span></span>|
|<span data-ttu-id="28e78-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="28e78-148">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-148">Int32</span></span>|<span data-ttu-id="28e78-149">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="28e78-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-150">errorDeviceCount</span></span>|<span data-ttu-id="28e78-151">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-151">Int32</span></span>|<span data-ttu-id="28e78-152">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-152">Number of error devices</span></span>|
|<span data-ttu-id="28e78-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-153">conflictDeviceCount</span></span>|<span data-ttu-id="28e78-154">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-154">Int32</span></span>|<span data-ttu-id="28e78-155">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-155">Number of conflict devices</span></span>|
|<span data-ttu-id="28e78-156">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e78-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="28e78-157">Int32</span><span class="sxs-lookup"><span data-stu-id="28e78-157">Int32</span></span>|<span data-ttu-id="28e78-158">未分配设备的数量</span><span class="sxs-lookup"><span data-stu-id="28e78-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="28e78-159">响应</span><span class="sxs-lookup"><span data-stu-id="28e78-159">Response</span></span>
<span data-ttu-id="28e78-160">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28e78-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e78-161">示例</span><span class="sxs-lookup"><span data-stu-id="28e78-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="28e78-162">请求</span><span class="sxs-lookup"><span data-stu-id="28e78-162">Request</span></span>
<span data-ttu-id="28e78-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28e78-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28e78-164">响应</span><span class="sxs-lookup"><span data-stu-id="28e78-164">Response</span></span>
<span data-ttu-id="28e78-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28e78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





