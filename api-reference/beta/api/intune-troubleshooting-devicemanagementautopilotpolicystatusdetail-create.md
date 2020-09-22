---
title: 创建 deviceManagementAutopilotPolicyStatusDetail
description: 创建新的 deviceManagementAutopilotPolicyStatusDetail 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7ea81e9099f3154d2139760bb310a8459ffa592
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999501"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="e108b-103">创建 deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="e108b-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="e108b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e108b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e108b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e108b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e108b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e108b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e108b-107">创建新的 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e108b-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e108b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e108b-108">Prerequisites</span></span>
<span data-ttu-id="e108b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e108b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e108b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e108b-111">Permission type</span></span>|<span data-ttu-id="e108b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e108b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e108b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e108b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e108b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e108b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e108b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e108b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e108b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e108b-116">Not supported.</span></span>|
|<span data-ttu-id="e108b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e108b-117">Application</span></span>|<span data-ttu-id="e108b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e108b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e108b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e108b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="e108b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e108b-120">Request headers</span></span>
|<span data-ttu-id="e108b-121">标头</span><span class="sxs-lookup"><span data-stu-id="e108b-121">Header</span></span>|<span data-ttu-id="e108b-122">值</span><span class="sxs-lookup"><span data-stu-id="e108b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e108b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e108b-123">Authorization</span></span>|<span data-ttu-id="e108b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e108b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e108b-125">接受</span><span class="sxs-lookup"><span data-stu-id="e108b-125">Accept</span></span>|<span data-ttu-id="e108b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e108b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e108b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e108b-127">Request body</span></span>
<span data-ttu-id="e108b-128">在请求正文中，提供 deviceManagementAutopilotPolicyStatusDetail 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e108b-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="e108b-129">下表显示创建 deviceManagementAutopilotPolicyStatusDetail 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e108b-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="e108b-130">属性</span><span class="sxs-lookup"><span data-stu-id="e108b-130">Property</span></span>|<span data-ttu-id="e108b-131">类型</span><span class="sxs-lookup"><span data-stu-id="e108b-131">Type</span></span>|<span data-ttu-id="e108b-132">说明</span><span class="sxs-lookup"><span data-stu-id="e108b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e108b-133">id</span><span class="sxs-lookup"><span data-stu-id="e108b-133">id</span></span>|<span data-ttu-id="e108b-134">String</span><span class="sxs-lookup"><span data-stu-id="e108b-134">String</span></span>|<span data-ttu-id="e108b-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="e108b-135">UUID for the object</span></span>|
|<span data-ttu-id="e108b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e108b-136">displayName</span></span>|<span data-ttu-id="e108b-137">String</span><span class="sxs-lookup"><span data-stu-id="e108b-137">String</span></span>|<span data-ttu-id="e108b-138">策略的友好名称。</span><span class="sxs-lookup"><span data-stu-id="e108b-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="e108b-139">policyType</span><span class="sxs-lookup"><span data-stu-id="e108b-139">policyType</span></span>|[<span data-ttu-id="e108b-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="e108b-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="e108b-141">策略的类型。</span><span class="sxs-lookup"><span data-stu-id="e108b-141">The type of policy.</span></span> <span data-ttu-id="e108b-142">可取值为：`unknown`、`application`、`appModel`、`configurationPolicy`。</span><span class="sxs-lookup"><span data-stu-id="e108b-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="e108b-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e108b-143">complianceStatus</span></span>|[<span data-ttu-id="e108b-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="e108b-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="e108b-145">策略合规性状态。</span><span class="sxs-lookup"><span data-stu-id="e108b-145">The policy compliance status.</span></span> <span data-ttu-id="e108b-146">可取值为：`unknown`、`compliant`、`installed`、`notCompliant`、`notInstalled`、`error`。</span><span class="sxs-lookup"><span data-stu-id="e108b-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="e108b-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="e108b-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="e108b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e108b-148">Boolean</span></span>|<span data-ttu-id="e108b-149">指示是否已将此 prolicy 作为 autopilot 引导注册同步会话的一部分进行跟踪</span><span class="sxs-lookup"><span data-stu-id="e108b-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="e108b-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e108b-150">lastReportedDateTime</span></span>|<span data-ttu-id="e108b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e108b-151">DateTimeOffset</span></span>|<span data-ttu-id="e108b-152">报告的策略状态的时间戳</span><span class="sxs-lookup"><span data-stu-id="e108b-152">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="e108b-153">响应</span><span class="sxs-lookup"><span data-stu-id="e108b-153">Response</span></span>
<span data-ttu-id="e108b-154">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e108b-154">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e108b-155">示例</span><span class="sxs-lookup"><span data-stu-id="e108b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="e108b-156">请求</span><span class="sxs-lookup"><span data-stu-id="e108b-156">Request</span></span>
<span data-ttu-id="e108b-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e108b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
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

### <a name="response"></a><span data-ttu-id="e108b-158">响应</span><span class="sxs-lookup"><span data-stu-id="e108b-158">Response</span></span>
<span data-ttu-id="e108b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e108b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






