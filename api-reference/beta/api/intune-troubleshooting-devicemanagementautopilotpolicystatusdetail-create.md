---
title: 创建 deviceManagementAutopilotPolicyStatusDetail
description: 创建新的 deviceManagementAutopilotPolicyStatusDetail 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3f2b6614d980911c35babfa71425a2e5b0ac7e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134193"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="e6753-103">创建 deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="e6753-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="e6753-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6753-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6753-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6753-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6753-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6753-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6753-107">创建新的 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6753-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6753-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6753-108">Prerequisites</span></span>
<span data-ttu-id="e6753-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6753-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6753-111">Permission type</span></span>|<span data-ttu-id="e6753-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6753-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6753-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6753-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6753-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6753-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e6753-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6753-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6753-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6753-116">Not supported.</span></span>|
|<span data-ttu-id="e6753-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6753-117">Application</span></span>|<span data-ttu-id="e6753-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6753-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6753-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6753-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="e6753-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6753-120">Request headers</span></span>
|<span data-ttu-id="e6753-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6753-121">Header</span></span>|<span data-ttu-id="e6753-122">值</span><span class="sxs-lookup"><span data-stu-id="e6753-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6753-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6753-123">Authorization</span></span>|<span data-ttu-id="e6753-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6753-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6753-125">接受</span><span class="sxs-lookup"><span data-stu-id="e6753-125">Accept</span></span>|<span data-ttu-id="e6753-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6753-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6753-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6753-127">Request body</span></span>
<span data-ttu-id="e6753-128">在请求正文中，提供 deviceManagementAutopilotPolicyStatusDetail 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6753-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="e6753-129">下表显示创建 deviceManagementAutopilotPolicyStatusDetail 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6753-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="e6753-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6753-130">Property</span></span>|<span data-ttu-id="e6753-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6753-131">Type</span></span>|<span data-ttu-id="e6753-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6753-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6753-133">id</span><span class="sxs-lookup"><span data-stu-id="e6753-133">id</span></span>|<span data-ttu-id="e6753-134">String</span><span class="sxs-lookup"><span data-stu-id="e6753-134">String</span></span>|<span data-ttu-id="e6753-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="e6753-135">UUID for the object</span></span>|
|<span data-ttu-id="e6753-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e6753-136">displayName</span></span>|<span data-ttu-id="e6753-137">String</span><span class="sxs-lookup"><span data-stu-id="e6753-137">String</span></span>|<span data-ttu-id="e6753-138">策略的友好名称。</span><span class="sxs-lookup"><span data-stu-id="e6753-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="e6753-139">policyType</span><span class="sxs-lookup"><span data-stu-id="e6753-139">policyType</span></span>|[<span data-ttu-id="e6753-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="e6753-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="e6753-141">策略的类型。</span><span class="sxs-lookup"><span data-stu-id="e6753-141">The type of policy.</span></span> <span data-ttu-id="e6753-142">可取值为：`unknown`、`application`、`appModel`、`configurationPolicy`。</span><span class="sxs-lookup"><span data-stu-id="e6753-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="e6753-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e6753-143">complianceStatus</span></span>|[<span data-ttu-id="e6753-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="e6753-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="e6753-145">策略合规性状态。</span><span class="sxs-lookup"><span data-stu-id="e6753-145">The policy compliance status.</span></span> <span data-ttu-id="e6753-146">可取值为：`unknown`、`compliant`、`installed`、`notCompliant`、`notInstalled`、`error`。</span><span class="sxs-lookup"><span data-stu-id="e6753-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="e6753-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="e6753-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="e6753-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6753-148">Boolean</span></span>|<span data-ttu-id="e6753-149">指示此许可是否作为 autopilot 启动注册同步会话的一部分进行跟踪</span><span class="sxs-lookup"><span data-stu-id="e6753-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="e6753-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6753-150">lastReportedDateTime</span></span>|<span data-ttu-id="e6753-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6753-151">DateTimeOffset</span></span>|<span data-ttu-id="e6753-152">报告的策略状态的时间戳</span><span class="sxs-lookup"><span data-stu-id="e6753-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="e6753-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="e6753-153">errorCode</span></span>|<span data-ttu-id="e6753-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e6753-154">Int32</span></span>|<span data-ttu-id="e6753-155">与策略的合规性或强制状态相关联的错误模式。</span><span class="sxs-lookup"><span data-stu-id="e6753-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="e6753-156">强制状态的错误代码如果存在，则优先。</span><span class="sxs-lookup"><span data-stu-id="e6753-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="e6753-157">响应</span><span class="sxs-lookup"><span data-stu-id="e6753-157">Response</span></span>
<span data-ttu-id="e6753-158">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6753-158">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6753-159">示例</span><span class="sxs-lookup"><span data-stu-id="e6753-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6753-160">请求</span><span class="sxs-lookup"><span data-stu-id="e6753-160">Request</span></span>
<span data-ttu-id="e6753-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6753-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```

### <a name="response"></a><span data-ttu-id="e6753-162">响应</span><span class="sxs-lookup"><span data-stu-id="e6753-162">Response</span></span>
<span data-ttu-id="e6753-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6753-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 363

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```




