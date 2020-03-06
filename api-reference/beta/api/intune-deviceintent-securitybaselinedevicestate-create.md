---
title: 创建 securityBaselineDeviceState
description: 创建新的 securityBaselineDeviceState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 618eb1f5395b004ecf62b4d3c22ba412886d754f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470229"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="946e7-103">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="946e7-103">Create securityBaselineDeviceState</span></span>

<span data-ttu-id="946e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="946e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="946e7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="946e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="946e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="946e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="946e7-107">创建新的[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="946e7-107">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="946e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="946e7-108">Prerequisites</span></span>
<span data-ttu-id="946e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="946e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="946e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="946e7-111">Permission type</span></span>|<span data-ttu-id="946e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="946e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="946e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="946e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="946e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="946e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="946e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="946e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="946e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="946e7-116">Not supported.</span></span>|
|<span data-ttu-id="946e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="946e7-117">Application</span></span>|<span data-ttu-id="946e7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="946e7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="946e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="946e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="946e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="946e7-120">Request headers</span></span>
|<span data-ttu-id="946e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="946e7-121">Header</span></span>|<span data-ttu-id="946e7-122">值</span><span class="sxs-lookup"><span data-stu-id="946e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="946e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="946e7-123">Authorization</span></span>|<span data-ttu-id="946e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="946e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="946e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="946e7-125">Accept</span></span>|<span data-ttu-id="946e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="946e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="946e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="946e7-127">Request body</span></span>
<span data-ttu-id="946e7-128">在请求正文中，提供 securityBaselineDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="946e7-128">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="946e7-129">下表显示创建 securityBaselineDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="946e7-129">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="946e7-130">属性</span><span class="sxs-lookup"><span data-stu-id="946e7-130">Property</span></span>|<span data-ttu-id="946e7-131">类型</span><span class="sxs-lookup"><span data-stu-id="946e7-131">Type</span></span>|<span data-ttu-id="946e7-132">说明</span><span class="sxs-lookup"><span data-stu-id="946e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="946e7-133">id</span><span class="sxs-lookup"><span data-stu-id="946e7-133">id</span></span>|<span data-ttu-id="946e7-134">String</span><span class="sxs-lookup"><span data-stu-id="946e7-134">String</span></span>|<span data-ttu-id="946e7-135">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="946e7-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="946e7-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="946e7-136">managedDeviceId</span></span>|<span data-ttu-id="946e7-137">字符串</span><span class="sxs-lookup"><span data-stu-id="946e7-137">String</span></span>|<span data-ttu-id="946e7-138">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="946e7-138">Intune device id</span></span>|
|<span data-ttu-id="946e7-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="946e7-139">deviceDisplayName</span></span>|<span data-ttu-id="946e7-140">String</span><span class="sxs-lookup"><span data-stu-id="946e7-140">String</span></span>|<span data-ttu-id="946e7-141">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="946e7-141">Display name of the device</span></span>|
|<span data-ttu-id="946e7-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="946e7-142">userPrincipalName</span></span>|<span data-ttu-id="946e7-143">字符串</span><span class="sxs-lookup"><span data-stu-id="946e7-143">String</span></span>|<span data-ttu-id="946e7-144">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="946e7-144">User Principal Name</span></span>|
|<span data-ttu-id="946e7-145">state</span><span class="sxs-lookup"><span data-stu-id="946e7-145">state</span></span>|[<span data-ttu-id="946e7-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="946e7-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="946e7-147">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="946e7-147">Security baseline compliance state.</span></span> <span data-ttu-id="946e7-148">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="946e7-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="946e7-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="946e7-149">lastReportedDateTime</span></span>|<span data-ttu-id="946e7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="946e7-150">DateTimeOffset</span></span>|<span data-ttu-id="946e7-151">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="946e7-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="946e7-152">响应</span><span class="sxs-lookup"><span data-stu-id="946e7-152">Response</span></span>
<span data-ttu-id="946e7-153">如果成功，此方法在响应`201 Created`正文中返回响应代码和[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="946e7-153">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="946e7-154">示例</span><span class="sxs-lookup"><span data-stu-id="946e7-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="946e7-155">请求</span><span class="sxs-lookup"><span data-stu-id="946e7-155">Request</span></span>
<span data-ttu-id="946e7-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="946e7-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="946e7-157">响应</span><span class="sxs-lookup"><span data-stu-id="946e7-157">Response</span></span>
<span data-ttu-id="946e7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="946e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 359

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "182749bf-49bf-1827-bf49-2718bf492718",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```





