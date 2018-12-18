---
title: 更新 advancedThreatProtectionOnboardingStateSummary
description: 更新 advancedThreatProtectionOnboardingStateSummary 对象的属性。
author: tfitzmac
ms.openlocfilehash: a31dae3c1f79332ae03324d1ecbb604451bc7959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340024"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="c8976-103">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8976-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="c8976-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c8976-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8976-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c8976-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8976-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c8976-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8976-107">更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8976-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8976-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8976-108">Prerequisites</span></span>
<span data-ttu-id="c8976-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c8976-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8976-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8976-111">Permission type</span></span>|<span data-ttu-id="c8976-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8976-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8976-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8976-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8976-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8976-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8976-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8976-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8976-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8976-116">Not supported.</span></span>|
|<span data-ttu-id="c8976-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8976-117">Application</span></span>|<span data-ttu-id="c8976-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8976-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8976-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8976-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c8976-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8976-120">Request headers</span></span>
|<span data-ttu-id="c8976-121">标头</span><span class="sxs-lookup"><span data-stu-id="c8976-121">Header</span></span>|<span data-ttu-id="c8976-122">值</span><span class="sxs-lookup"><span data-stu-id="c8976-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8976-123">授权</span><span class="sxs-lookup"><span data-stu-id="c8976-123">Authorization</span></span>|<span data-ttu-id="c8976-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8976-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8976-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8976-125">Accept</span></span>|<span data-ttu-id="c8976-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8976-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8976-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8976-127">Request body</span></span>
<span data-ttu-id="c8976-128">在请求正文中，提供[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8976-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="c8976-129">下表显示时创建[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c8976-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="c8976-130">属性</span><span class="sxs-lookup"><span data-stu-id="c8976-130">Property</span></span>|<span data-ttu-id="c8976-131">类型</span><span class="sxs-lookup"><span data-stu-id="c8976-131">Type</span></span>|<span data-ttu-id="c8976-132">说明</span><span class="sxs-lookup"><span data-stu-id="c8976-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8976-133">id</span><span class="sxs-lookup"><span data-stu-id="c8976-133">id</span></span>|<span data-ttu-id="c8976-134">String</span><span class="sxs-lookup"><span data-stu-id="c8976-134">String</span></span>|<span data-ttu-id="c8976-135">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="c8976-135">Unique Identifier</span></span>|
|<span data-ttu-id="c8976-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-136">unknownDeviceCount</span></span>|<span data-ttu-id="c8976-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-137">Int32</span></span>|<span data-ttu-id="c8976-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-138">Number of unknown devices</span></span>|
|<span data-ttu-id="c8976-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="c8976-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-140">Int32</span></span>|<span data-ttu-id="c8976-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="c8976-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-142">compliantDeviceCount</span></span>|<span data-ttu-id="c8976-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-143">Int32</span></span>|<span data-ttu-id="c8976-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-144">Number of compliant devices</span></span>|
|<span data-ttu-id="c8976-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-145">remediatedDeviceCount</span></span>|<span data-ttu-id="c8976-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-146">Int32</span></span>|<span data-ttu-id="c8976-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-147">Number of remediated devices</span></span>|
|<span data-ttu-id="c8976-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c8976-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-149">Int32</span></span>|<span data-ttu-id="c8976-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c8976-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-151">errorDeviceCount</span></span>|<span data-ttu-id="c8976-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-152">Int32</span></span>|<span data-ttu-id="c8976-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-153">Number of error devices</span></span>|
|<span data-ttu-id="c8976-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-154">conflictDeviceCount</span></span>|<span data-ttu-id="c8976-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-155">Int32</span></span>|<span data-ttu-id="c8976-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="c8976-156">Number of conflict devices</span></span>|
|<span data-ttu-id="c8976-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8976-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="c8976-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c8976-158">Int32</span></span>|<span data-ttu-id="c8976-159">未分配的设备数</span><span class="sxs-lookup"><span data-stu-id="c8976-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="c8976-160">响应</span><span class="sxs-lookup"><span data-stu-id="c8976-160">Response</span></span>
<span data-ttu-id="c8976-161">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8976-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8976-162">示例</span><span class="sxs-lookup"><span data-stu-id="c8976-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8976-163">请求</span><span class="sxs-lookup"><span data-stu-id="c8976-163">Request</span></span>
<span data-ttu-id="c8976-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8976-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 246

{
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

### <a name="response"></a><span data-ttu-id="c8976-165">响应</span><span class="sxs-lookup"><span data-stu-id="c8976-165">Response</span></span>
<span data-ttu-id="c8976-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8976-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





