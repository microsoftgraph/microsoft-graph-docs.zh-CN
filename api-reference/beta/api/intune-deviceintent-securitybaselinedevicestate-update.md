---
title: 更新 securityBaselineDeviceState
description: 更新 securityBaselineDeviceState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a0fd8ad1e7e357c0888dec4710bf912c0cdd1dc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945359"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="3acf5-103">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="3acf5-103">Update securityBaselineDeviceState</span></span>

> <span data-ttu-id="3acf5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3acf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3acf5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3acf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3acf5-106">更新[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3acf5-106">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3acf5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3acf5-107">Prerequisites</span></span>
<span data-ttu-id="3acf5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3acf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3acf5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3acf5-110">Permission type</span></span>|<span data-ttu-id="3acf5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3acf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3acf5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3acf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3acf5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acf5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3acf5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3acf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3acf5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3acf5-115">Not supported.</span></span>|
|<span data-ttu-id="3acf5-116">Application</span><span class="sxs-lookup"><span data-stu-id="3acf5-116">Application</span></span>|<span data-ttu-id="3acf5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acf5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3acf5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3acf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3acf5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3acf5-119">Request headers</span></span>
|<span data-ttu-id="3acf5-120">标头</span><span class="sxs-lookup"><span data-stu-id="3acf5-120">Header</span></span>|<span data-ttu-id="3acf5-121">值</span><span class="sxs-lookup"><span data-stu-id="3acf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3acf5-122">授权</span><span class="sxs-lookup"><span data-stu-id="3acf5-122">Authorization</span></span>|<span data-ttu-id="3acf5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3acf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3acf5-124">接受</span><span class="sxs-lookup"><span data-stu-id="3acf5-124">Accept</span></span>|<span data-ttu-id="3acf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3acf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3acf5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3acf5-126">Request body</span></span>
<span data-ttu-id="3acf5-127">在请求正文中，提供[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3acf5-127">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="3acf5-128">下表显示创建[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3acf5-128">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="3acf5-129">属性</span><span class="sxs-lookup"><span data-stu-id="3acf5-129">Property</span></span>|<span data-ttu-id="3acf5-130">类型</span><span class="sxs-lookup"><span data-stu-id="3acf5-130">Type</span></span>|<span data-ttu-id="3acf5-131">说明</span><span class="sxs-lookup"><span data-stu-id="3acf5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3acf5-132">id</span><span class="sxs-lookup"><span data-stu-id="3acf5-132">id</span></span>|<span data-ttu-id="3acf5-133">String</span><span class="sxs-lookup"><span data-stu-id="3acf5-133">String</span></span>|<span data-ttu-id="3acf5-134">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3acf5-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="3acf5-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="3acf5-135">managedDeviceId</span></span>|<span data-ttu-id="3acf5-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3acf5-136">String</span></span>|<span data-ttu-id="3acf5-137">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="3acf5-137">Intune device id</span></span>|
|<span data-ttu-id="3acf5-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3acf5-138">deviceDisplayName</span></span>|<span data-ttu-id="3acf5-139">String</span><span class="sxs-lookup"><span data-stu-id="3acf5-139">String</span></span>|<span data-ttu-id="3acf5-140">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="3acf5-140">Display name of the device</span></span>|
|<span data-ttu-id="3acf5-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3acf5-141">userPrincipalName</span></span>|<span data-ttu-id="3acf5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="3acf5-142">String</span></span>|<span data-ttu-id="3acf5-143">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="3acf5-143">User Principal Name</span></span>|
|<span data-ttu-id="3acf5-144">state</span><span class="sxs-lookup"><span data-stu-id="3acf5-144">state</span></span>|[<span data-ttu-id="3acf5-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="3acf5-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="3acf5-146">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="3acf5-146">Security baseline compliance state.</span></span> <span data-ttu-id="3acf5-147">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="3acf5-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="3acf5-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3acf5-148">lastReportedDateTime</span></span>|<span data-ttu-id="3acf5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acf5-149">DateTimeOffset</span></span>|<span data-ttu-id="3acf5-150">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="3acf5-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="3acf5-151">响应</span><span class="sxs-lookup"><span data-stu-id="3acf5-151">Response</span></span>
<span data-ttu-id="3acf5-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3acf5-152">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3acf5-153">示例</span><span class="sxs-lookup"><span data-stu-id="3acf5-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="3acf5-154">请求</span><span class="sxs-lookup"><span data-stu-id="3acf5-154">Request</span></span>
<span data-ttu-id="3acf5-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3acf5-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="3acf5-156">响应</span><span class="sxs-lookup"><span data-stu-id="3acf5-156">Response</span></span>
<span data-ttu-id="3acf5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3acf5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





