---
title: 创建 deviceManagementAutopilotPolicyStatusDetail
description: 创建新的 deviceManagementAutopilotPolicyStatusDetail 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a4a1680ec58e52d920a1cea8bf6772974bbb8f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299924"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="fdd1a-103">创建 deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="fdd1a-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="fdd1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdd1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdd1a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdd1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdd1a-107">创建新的 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdd1a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fdd1a-108">Prerequisites</span></span>
<span data-ttu-id="fdd1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdd1a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdd1a-111">Permission type</span></span>|<span data-ttu-id="fdd1a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fdd1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdd1a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdd1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdd1a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd1a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fdd1a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdd1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdd1a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-116">Not supported.</span></span>|
|<span data-ttu-id="fdd1a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdd1a-117">Application</span></span>|<span data-ttu-id="fdd1a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd1a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdd1a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdd1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="fdd1a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdd1a-120">Request headers</span></span>
|<span data-ttu-id="fdd1a-121">标头</span><span class="sxs-lookup"><span data-stu-id="fdd1a-121">Header</span></span>|<span data-ttu-id="fdd1a-122">值</span><span class="sxs-lookup"><span data-stu-id="fdd1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdd1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdd1a-123">Authorization</span></span>|<span data-ttu-id="fdd1a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdd1a-125">接受</span><span class="sxs-lookup"><span data-stu-id="fdd1a-125">Accept</span></span>|<span data-ttu-id="fdd1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdd1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdd1a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdd1a-127">Request body</span></span>
<span data-ttu-id="fdd1a-128">在请求正文中，提供 deviceManagementAutopilotPolicyStatusDetail 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="fdd1a-129">下表显示创建 deviceManagementAutopilotPolicyStatusDetail 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="fdd1a-130">属性</span><span class="sxs-lookup"><span data-stu-id="fdd1a-130">Property</span></span>|<span data-ttu-id="fdd1a-131">类型</span><span class="sxs-lookup"><span data-stu-id="fdd1a-131">Type</span></span>|<span data-ttu-id="fdd1a-132">说明</span><span class="sxs-lookup"><span data-stu-id="fdd1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdd1a-133">id</span><span class="sxs-lookup"><span data-stu-id="fdd1a-133">id</span></span>|<span data-ttu-id="fdd1a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="fdd1a-134">String</span></span>|<span data-ttu-id="fdd1a-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="fdd1a-135">UUID for the object</span></span>|
|<span data-ttu-id="fdd1a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fdd1a-136">displayName</span></span>|<span data-ttu-id="fdd1a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="fdd1a-137">String</span></span>|<span data-ttu-id="fdd1a-138">策略的友好名称。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="fdd1a-139">policyType</span><span class="sxs-lookup"><span data-stu-id="fdd1a-139">policyType</span></span>|[<span data-ttu-id="fdd1a-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="fdd1a-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="fdd1a-141">策略的类型。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-141">The type of policy.</span></span> <span data-ttu-id="fdd1a-142">可取值为：`unknown`、`application`、`appModel`、`configurationPolicy`。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="fdd1a-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fdd1a-143">complianceStatus</span></span>|[<span data-ttu-id="fdd1a-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="fdd1a-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="fdd1a-145">策略合规性状态。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-145">The policy compliance status.</span></span> <span data-ttu-id="fdd1a-146">可取值为：`unknown`、`compliant`、`installed`、`notCompliant`、`notInstalled`、`error`。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="fdd1a-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="fdd1a-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="fdd1a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdd1a-148">Boolean</span></span>|<span data-ttu-id="fdd1a-149">指示是否已将此 prolicy 作为 autopilot 引导注册同步会话的一部分进行跟踪</span><span class="sxs-lookup"><span data-stu-id="fdd1a-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="fdd1a-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdd1a-150">lastReportedDateTime</span></span>|<span data-ttu-id="fdd1a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdd1a-151">DateTimeOffset</span></span>|<span data-ttu-id="fdd1a-152">报告的策略状态的时间戳</span><span class="sxs-lookup"><span data-stu-id="fdd1a-152">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="fdd1a-153">响应</span><span class="sxs-lookup"><span data-stu-id="fdd1a-153">Response</span></span>
<span data-ttu-id="fdd1a-154">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-154">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdd1a-155">示例</span><span class="sxs-lookup"><span data-stu-id="fdd1a-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdd1a-156">请求</span><span class="sxs-lookup"><span data-stu-id="fdd1a-156">Request</span></span>
<span data-ttu-id="fdd1a-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdd1a-158">响应</span><span class="sxs-lookup"><span data-stu-id="fdd1a-158">Response</span></span>
<span data-ttu-id="fdd1a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fdd1a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




