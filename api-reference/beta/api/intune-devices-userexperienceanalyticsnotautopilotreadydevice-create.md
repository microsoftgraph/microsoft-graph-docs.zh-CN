---
title: 创建 userExperienceAnalyticsNotAutopilotReadyDevice
description: 创建新的 userExperienceAnalyticsNotAutopilotReadyDevice 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1473c0a856636dc5373239c1bed4c2caed9ea78b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865220"
---
# <a name="create-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="574d2-103">创建 userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="574d2-103">Create userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="574d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="574d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="574d2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="574d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="574d2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="574d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="574d2-107">创建新的 [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="574d2-107">Create a new [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="574d2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="574d2-108">Prerequisites</span></span>
<span data-ttu-id="574d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="574d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="574d2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="574d2-111">Permission type</span></span>|<span data-ttu-id="574d2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="574d2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="574d2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="574d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="574d2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="574d2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="574d2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="574d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="574d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="574d2-116">Not supported.</span></span>|
|<span data-ttu-id="574d2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="574d2-117">Application</span></span>|<span data-ttu-id="574d2-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="574d2-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="574d2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="574d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="574d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="574d2-120">Request headers</span></span>
|<span data-ttu-id="574d2-121">标头</span><span class="sxs-lookup"><span data-stu-id="574d2-121">Header</span></span>|<span data-ttu-id="574d2-122">值</span><span class="sxs-lookup"><span data-stu-id="574d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="574d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="574d2-123">Authorization</span></span>|<span data-ttu-id="574d2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="574d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="574d2-125">接受</span><span class="sxs-lookup"><span data-stu-id="574d2-125">Accept</span></span>|<span data-ttu-id="574d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="574d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="574d2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="574d2-127">Request body</span></span>
<span data-ttu-id="574d2-128">在请求正文中，提供 userExperienceAnalyticsNotAutopilotReadyDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="574d2-128">In the request body, supply a JSON representation for the userExperienceAnalyticsNotAutopilotReadyDevice object.</span></span>

<span data-ttu-id="574d2-129">下表显示创建 userExperienceAnalyticsNotAutopilotReadyDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="574d2-129">The following table shows the properties that are required when you create the userExperienceAnalyticsNotAutopilotReadyDevice.</span></span>

|<span data-ttu-id="574d2-130">属性</span><span class="sxs-lookup"><span data-stu-id="574d2-130">Property</span></span>|<span data-ttu-id="574d2-131">类型</span><span class="sxs-lookup"><span data-stu-id="574d2-131">Type</span></span>|<span data-ttu-id="574d2-132">说明</span><span class="sxs-lookup"><span data-stu-id="574d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="574d2-133">id</span><span class="sxs-lookup"><span data-stu-id="574d2-133">id</span></span>|<span data-ttu-id="574d2-134">String</span><span class="sxs-lookup"><span data-stu-id="574d2-134">String</span></span>|<span data-ttu-id="574d2-135">用户体验分析 intune 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="574d2-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="574d2-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="574d2-136">deviceName</span></span>|<span data-ttu-id="574d2-137">String</span><span class="sxs-lookup"><span data-stu-id="574d2-137">String</span></span>|<span data-ttu-id="574d2-138">intune 设备的名称。</span><span class="sxs-lookup"><span data-stu-id="574d2-138">The intune device's name.</span></span>|
|<span data-ttu-id="574d2-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="574d2-139">serialNumber</span></span>|<span data-ttu-id="574d2-140">String</span><span class="sxs-lookup"><span data-stu-id="574d2-140">String</span></span>|<span data-ttu-id="574d2-141">intune 设备的序列号。</span><span class="sxs-lookup"><span data-stu-id="574d2-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="574d2-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="574d2-142">manufacturer</span></span>|<span data-ttu-id="574d2-143">String</span><span class="sxs-lookup"><span data-stu-id="574d2-143">String</span></span>|<span data-ttu-id="574d2-144">intune 设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="574d2-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="574d2-145">model</span><span class="sxs-lookup"><span data-stu-id="574d2-145">model</span></span>|<span data-ttu-id="574d2-146">String</span><span class="sxs-lookup"><span data-stu-id="574d2-146">String</span></span>|<span data-ttu-id="574d2-147">intune 设备的型号。</span><span class="sxs-lookup"><span data-stu-id="574d2-147">The intune device's model.</span></span>|
|<span data-ttu-id="574d2-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="574d2-148">managedBy</span></span>|<span data-ttu-id="574d2-149">String</span><span class="sxs-lookup"><span data-stu-id="574d2-149">String</span></span>|<span data-ttu-id="574d2-150">intune 设备的托管者。</span><span class="sxs-lookup"><span data-stu-id="574d2-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="574d2-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="574d2-151">autoPilotRegistered</span></span>|<span data-ttu-id="574d2-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="574d2-152">Boolean</span></span>|<span data-ttu-id="574d2-153">intune 设备的 autopilotRegistered。</span><span class="sxs-lookup"><span data-stu-id="574d2-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="574d2-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="574d2-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="574d2-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="574d2-155">Boolean</span></span>|<span data-ttu-id="574d2-156">intune 设备的 autopilotProfileAssigned。</span><span class="sxs-lookup"><span data-stu-id="574d2-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="574d2-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="574d2-157">azureAdRegistered</span></span>|<span data-ttu-id="574d2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="574d2-158">Boolean</span></span>|<span data-ttu-id="574d2-159">intune 设备的 azureAdRegistered。</span><span class="sxs-lookup"><span data-stu-id="574d2-159">The intune device's azureAdRegistered.</span></span>|
|<span data-ttu-id="574d2-160">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="574d2-160">azureAdJoinType</span></span>|<span data-ttu-id="574d2-161">String</span><span class="sxs-lookup"><span data-stu-id="574d2-161">String</span></span>|<span data-ttu-id="574d2-162">intune 设备的 azure Ad joinType。</span><span class="sxs-lookup"><span data-stu-id="574d2-162">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="574d2-163">响应</span><span class="sxs-lookup"><span data-stu-id="574d2-163">Response</span></span>
<span data-ttu-id="574d2-164">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="574d2-164">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="574d2-165">示例</span><span class="sxs-lookup"><span data-stu-id="574d2-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="574d2-166">请求</span><span class="sxs-lookup"><span data-stu-id="574d2-166">Request</span></span>
<span data-ttu-id="574d2-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="574d2-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="574d2-168">响应</span><span class="sxs-lookup"><span data-stu-id="574d2-168">Response</span></span>
<span data-ttu-id="574d2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="574d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




