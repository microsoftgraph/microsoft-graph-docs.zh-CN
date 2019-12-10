---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95b43a19625b4501d385c683cb463f32ed42def0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938521"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="47e9f-103">更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="47e9f-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

> <span data-ttu-id="47e9f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47e9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47e9f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47e9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47e9f-106">更新[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47e9f-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47e9f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="47e9f-107">Prerequisites</span></span>
<span data-ttu-id="47e9f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47e9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47e9f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="47e9f-110">Permission type</span></span>|<span data-ttu-id="47e9f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="47e9f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47e9f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47e9f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47e9f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e9f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47e9f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47e9f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47e9f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="47e9f-115">Not supported.</span></span>|
|<span data-ttu-id="47e9f-116">Application</span><span class="sxs-lookup"><span data-stu-id="47e9f-116">Application</span></span>|<span data-ttu-id="47e9f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e9f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47e9f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47e9f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="47e9f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="47e9f-119">Request headers</span></span>
|<span data-ttu-id="47e9f-120">标头</span><span class="sxs-lookup"><span data-stu-id="47e9f-120">Header</span></span>|<span data-ttu-id="47e9f-121">值</span><span class="sxs-lookup"><span data-stu-id="47e9f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47e9f-122">授权</span><span class="sxs-lookup"><span data-stu-id="47e9f-122">Authorization</span></span>|<span data-ttu-id="47e9f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47e9f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47e9f-124">接受</span><span class="sxs-lookup"><span data-stu-id="47e9f-124">Accept</span></span>|<span data-ttu-id="47e9f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47e9f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47e9f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="47e9f-126">Request body</span></span>
<span data-ttu-id="47e9f-127">在请求正文中，提供[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47e9f-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="47e9f-128">下表显示创建[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="47e9f-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="47e9f-129">属性</span><span class="sxs-lookup"><span data-stu-id="47e9f-129">Property</span></span>|<span data-ttu-id="47e9f-130">类型</span><span class="sxs-lookup"><span data-stu-id="47e9f-130">Type</span></span>|<span data-ttu-id="47e9f-131">说明</span><span class="sxs-lookup"><span data-stu-id="47e9f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e9f-132">id</span><span class="sxs-lookup"><span data-stu-id="47e9f-132">id</span></span>|<span data-ttu-id="47e9f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="47e9f-133">String</span></span>|<span data-ttu-id="47e9f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47e9f-134">Key of the entity.</span></span>|
|<span data-ttu-id="47e9f-135">deployedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47e9f-135">deployedDeviceCount</span></span>|<span data-ttu-id="47e9f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="47e9f-136">Int32</span></span>|<span data-ttu-id="47e9f-137">已成功部署此 WindowsDefenderApplicationControl 补充策略的设备数量。</span><span class="sxs-lookup"><span data-stu-id="47e9f-137">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="47e9f-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47e9f-138">failedDeviceCount</span></span>|<span data-ttu-id="47e9f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="47e9f-139">Int32</span></span>|<span data-ttu-id="47e9f-140">无法部署此 WindowsDefenderApplicationControl 补充策略的设备数量。</span><span class="sxs-lookup"><span data-stu-id="47e9f-140">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="47e9f-141">响应</span><span class="sxs-lookup"><span data-stu-id="47e9f-141">Response</span></span>
<span data-ttu-id="47e9f-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47e9f-142">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47e9f-143">示例</span><span class="sxs-lookup"><span data-stu-id="47e9f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="47e9f-144">请求</span><span class="sxs-lookup"><span data-stu-id="47e9f-144">Request</span></span>
<span data-ttu-id="47e9f-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47e9f-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "deployedDeviceCount": 3,
  "failedDeviceCount": 1
}
```

### <a name="response"></a><span data-ttu-id="47e9f-146">响应</span><span class="sxs-lookup"><span data-stu-id="47e9f-146">Response</span></span>
<span data-ttu-id="47e9f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47e9f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "2f8656ed-56ed-2f86-ed56-862fed56862f",
  "deployedDeviceCount": 3,
  "failedDeviceCount": 1
}
```





