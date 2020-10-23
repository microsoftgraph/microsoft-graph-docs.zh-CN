---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be2dcb687b79798bede22930cbaed1cb49e95d61
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724015"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="b8e4b-103">更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="b8e4b-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

<span data-ttu-id="b8e4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8e4b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8e4b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e4b-107">更新 [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8e4b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8e4b-108">Prerequisites</span></span>
<span data-ttu-id="b8e4b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8e4b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8e4b-111">Permission type</span></span>|<span data-ttu-id="b8e4b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8e4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8e4b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8e4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8e4b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e4b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8e4b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8e4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8e4b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-116">Not supported.</span></span>|
|<span data-ttu-id="b8e4b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8e4b-117">Application</span></span>|<span data-ttu-id="b8e4b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e4b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8e4b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8e4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="b8e4b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8e4b-120">Request headers</span></span>
|<span data-ttu-id="b8e4b-121">标头</span><span class="sxs-lookup"><span data-stu-id="b8e4b-121">Header</span></span>|<span data-ttu-id="b8e4b-122">值</span><span class="sxs-lookup"><span data-stu-id="b8e4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8e4b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8e4b-123">Authorization</span></span>|<span data-ttu-id="b8e4b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8e4b-125">接受</span><span class="sxs-lookup"><span data-stu-id="b8e4b-125">Accept</span></span>|<span data-ttu-id="b8e4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8e4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8e4b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8e4b-127">Request body</span></span>
<span data-ttu-id="b8e4b-128">在请求正文中，提供 [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="b8e4b-129">下表显示创建 [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="b8e4b-130">属性</span><span class="sxs-lookup"><span data-stu-id="b8e4b-130">Property</span></span>|<span data-ttu-id="b8e4b-131">类型</span><span class="sxs-lookup"><span data-stu-id="b8e4b-131">Type</span></span>|<span data-ttu-id="b8e4b-132">说明</span><span class="sxs-lookup"><span data-stu-id="b8e4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e4b-133">id</span><span class="sxs-lookup"><span data-stu-id="b8e4b-133">id</span></span>|<span data-ttu-id="b8e4b-134">String</span><span class="sxs-lookup"><span data-stu-id="b8e4b-134">String</span></span>|<span data-ttu-id="b8e4b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-135">Key of the entity.</span></span>|
|<span data-ttu-id="b8e4b-136">deployedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8e4b-136">deployedDeviceCount</span></span>|<span data-ttu-id="b8e4b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e4b-137">Int32</span></span>|<span data-ttu-id="b8e4b-138">已成功部署此 WindowsDefenderApplicationControl 补充策略的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-138">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="b8e4b-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8e4b-139">failedDeviceCount</span></span>|<span data-ttu-id="b8e4b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e4b-140">Int32</span></span>|<span data-ttu-id="b8e4b-141">无法部署此 WindowsDefenderApplicationControl 补充策略的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-141">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="b8e4b-142">响应</span><span class="sxs-lookup"><span data-stu-id="b8e4b-142">Response</span></span>
<span data-ttu-id="b8e4b-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-143">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8e4b-144">示例</span><span class="sxs-lookup"><span data-stu-id="b8e4b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8e4b-145">请求</span><span class="sxs-lookup"><span data-stu-id="b8e4b-145">Request</span></span>
<span data-ttu-id="b8e4b-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8e4b-147">响应</span><span class="sxs-lookup"><span data-stu-id="b8e4b-147">Response</span></span>
<span data-ttu-id="b8e4b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8e4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





