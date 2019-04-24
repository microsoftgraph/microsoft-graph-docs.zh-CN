---
title: 创建 securityBaselineDeviceState
description: 创建新的 securityBaselineDeviceState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0b816fb81d85536dcb220b5cb7fc3483549ab85
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466600"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="cfd77-103">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="cfd77-103">Create securityBaselineDeviceState</span></span>

> <span data-ttu-id="cfd77-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cfd77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfd77-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cfd77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfd77-106">创建新的[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cfd77-106">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfd77-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cfd77-107">Prerequisites</span></span>
<span data-ttu-id="cfd77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfd77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfd77-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfd77-110">Permission type</span></span>|<span data-ttu-id="cfd77-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cfd77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfd77-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfd77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfd77-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd77-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfd77-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfd77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfd77-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfd77-115">Not supported.</span></span>|
|<span data-ttu-id="cfd77-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfd77-116">Application</span></span>|<span data-ttu-id="cfd77-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfd77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfd77-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfd77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="cfd77-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfd77-119">Request headers</span></span>
|<span data-ttu-id="cfd77-120">标头</span><span class="sxs-lookup"><span data-stu-id="cfd77-120">Header</span></span>|<span data-ttu-id="cfd77-121">值</span><span class="sxs-lookup"><span data-stu-id="cfd77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfd77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfd77-122">Authorization</span></span>|<span data-ttu-id="cfd77-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cfd77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfd77-124">接受</span><span class="sxs-lookup"><span data-stu-id="cfd77-124">Accept</span></span>|<span data-ttu-id="cfd77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfd77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfd77-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfd77-126">Request body</span></span>
<span data-ttu-id="cfd77-127">在请求正文中, 提供 securityBaselineDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfd77-127">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="cfd77-128">下表显示创建 securityBaselineDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cfd77-128">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="cfd77-129">属性</span><span class="sxs-lookup"><span data-stu-id="cfd77-129">Property</span></span>|<span data-ttu-id="cfd77-130">类型</span><span class="sxs-lookup"><span data-stu-id="cfd77-130">Type</span></span>|<span data-ttu-id="cfd77-131">说明</span><span class="sxs-lookup"><span data-stu-id="cfd77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfd77-132">id</span><span class="sxs-lookup"><span data-stu-id="cfd77-132">id</span></span>|<span data-ttu-id="cfd77-133">String</span><span class="sxs-lookup"><span data-stu-id="cfd77-133">String</span></span>|<span data-ttu-id="cfd77-134">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cfd77-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="cfd77-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="cfd77-135">managedDeviceId</span></span>|<span data-ttu-id="cfd77-136">字符串</span><span class="sxs-lookup"><span data-stu-id="cfd77-136">String</span></span>|<span data-ttu-id="cfd77-137">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="cfd77-137">Intune device id</span></span>|
|<span data-ttu-id="cfd77-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cfd77-138">deviceDisplayName</span></span>|<span data-ttu-id="cfd77-139">String</span><span class="sxs-lookup"><span data-stu-id="cfd77-139">String</span></span>|<span data-ttu-id="cfd77-140">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="cfd77-140">Display name of the device</span></span>|
|<span data-ttu-id="cfd77-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cfd77-141">userPrincipalName</span></span>|<span data-ttu-id="cfd77-142">String</span><span class="sxs-lookup"><span data-stu-id="cfd77-142">String</span></span>|<span data-ttu-id="cfd77-143">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="cfd77-143">User Principal Name</span></span>|
|<span data-ttu-id="cfd77-144">state</span><span class="sxs-lookup"><span data-stu-id="cfd77-144">state</span></span>|[<span data-ttu-id="cfd77-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="cfd77-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="cfd77-146">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="cfd77-146">Security baseline compliance state.</span></span> <span data-ttu-id="cfd77-147">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="cfd77-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="cfd77-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfd77-148">lastReportedDateTime</span></span>|<span data-ttu-id="cfd77-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfd77-149">DateTimeOffset</span></span>|<span data-ttu-id="cfd77-150">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="cfd77-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="cfd77-151">响应</span><span class="sxs-lookup"><span data-stu-id="cfd77-151">Response</span></span>
<span data-ttu-id="cfd77-152">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cfd77-152">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfd77-153">示例</span><span class="sxs-lookup"><span data-stu-id="cfd77-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfd77-154">请求</span><span class="sxs-lookup"><span data-stu-id="cfd77-154">Request</span></span>
<span data-ttu-id="cfd77-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfd77-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cfd77-156">响应</span><span class="sxs-lookup"><span data-stu-id="cfd77-156">Response</span></span>
<span data-ttu-id="cfd77-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cfd77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





