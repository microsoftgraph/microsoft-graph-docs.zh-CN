---
title: 更新 deviceManagementAutopilotPolicyStatusDetail
description: 更新 deviceManagementAutopilotPolicyStatusDetail 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c3c94dcde401fb4917171e97b18995bf2c6cf07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800198"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="5806b-103">更新 deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="5806b-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

> <span data-ttu-id="5806b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5806b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5806b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5806b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5806b-106">更新[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5806b-106">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5806b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5806b-107">Prerequisites</span></span>
<span data-ttu-id="5806b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5806b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5806b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5806b-110">Permission type</span></span>|<span data-ttu-id="5806b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5806b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5806b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5806b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5806b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5806b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5806b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5806b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5806b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5806b-115">Not supported.</span></span>|
|<span data-ttu-id="5806b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5806b-116">Application</span></span>|<span data-ttu-id="5806b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5806b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5806b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5806b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="5806b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5806b-119">Request headers</span></span>
|<span data-ttu-id="5806b-120">标头</span><span class="sxs-lookup"><span data-stu-id="5806b-120">Header</span></span>|<span data-ttu-id="5806b-121">值</span><span class="sxs-lookup"><span data-stu-id="5806b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5806b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5806b-122">Authorization</span></span>|<span data-ttu-id="5806b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5806b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5806b-124">接受</span><span class="sxs-lookup"><span data-stu-id="5806b-124">Accept</span></span>|<span data-ttu-id="5806b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5806b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5806b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5806b-126">Request body</span></span>
<span data-ttu-id="5806b-127">在请求正文中，提供[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5806b-127">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="5806b-128">下表显示创建[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5806b-128">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="5806b-129">属性</span><span class="sxs-lookup"><span data-stu-id="5806b-129">Property</span></span>|<span data-ttu-id="5806b-130">类型</span><span class="sxs-lookup"><span data-stu-id="5806b-130">Type</span></span>|<span data-ttu-id="5806b-131">说明</span><span class="sxs-lookup"><span data-stu-id="5806b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5806b-132">id</span><span class="sxs-lookup"><span data-stu-id="5806b-132">id</span></span>|<span data-ttu-id="5806b-133">String</span><span class="sxs-lookup"><span data-stu-id="5806b-133">String</span></span>|<span data-ttu-id="5806b-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="5806b-134">UUID for the object</span></span>|
|<span data-ttu-id="5806b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5806b-135">displayName</span></span>|<span data-ttu-id="5806b-136">String</span><span class="sxs-lookup"><span data-stu-id="5806b-136">String</span></span>|<span data-ttu-id="5806b-137">策略的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5806b-137">The friendly name of the policy.</span></span>|
|<span data-ttu-id="5806b-138">policyType</span><span class="sxs-lookup"><span data-stu-id="5806b-138">policyType</span></span>|[<span data-ttu-id="5806b-139">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="5806b-139">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="5806b-140">策略的类型。</span><span class="sxs-lookup"><span data-stu-id="5806b-140">The type of policy.</span></span> <span data-ttu-id="5806b-141">可取值为：`unknown`、`application`、`appModel`、`configurationPolicy`。</span><span class="sxs-lookup"><span data-stu-id="5806b-141">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="5806b-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5806b-142">complianceStatus</span></span>|[<span data-ttu-id="5806b-143">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="5806b-143">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="5806b-144">策略合规性状态。</span><span class="sxs-lookup"><span data-stu-id="5806b-144">The policy compliance status.</span></span> <span data-ttu-id="5806b-145">可取值为：`unknown`、`compliant`、`installed`、`notCompliant`、`notInstalled`、`error`。</span><span class="sxs-lookup"><span data-stu-id="5806b-145">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="5806b-146">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="5806b-146">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="5806b-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="5806b-147">Boolean</span></span>|<span data-ttu-id="5806b-148">指示是否已将此 prolicy 作为 autopilot 引导注册同步会话的一部分进行跟踪</span><span class="sxs-lookup"><span data-stu-id="5806b-148">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="5806b-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5806b-149">lastReportedDateTime</span></span>|<span data-ttu-id="5806b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5806b-150">DateTimeOffset</span></span>|<span data-ttu-id="5806b-151">报告的策略状态的时间戳</span><span class="sxs-lookup"><span data-stu-id="5806b-151">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="5806b-152">响应</span><span class="sxs-lookup"><span data-stu-id="5806b-152">Response</span></span>
<span data-ttu-id="5806b-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5806b-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5806b-154">示例</span><span class="sxs-lookup"><span data-stu-id="5806b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="5806b-155">请求</span><span class="sxs-lookup"><span data-stu-id="5806b-155">Request</span></span>
<span data-ttu-id="5806b-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5806b-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5806b-157">响应</span><span class="sxs-lookup"><span data-stu-id="5806b-157">Response</span></span>
<span data-ttu-id="5806b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5806b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




