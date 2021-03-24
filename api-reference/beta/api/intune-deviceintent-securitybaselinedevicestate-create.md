---
title: 创建 securityBaselineDeviceState
description: 创建新的 securityBaselineDeviceState 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 498c9799315ba844001c82058915e8b0ec68a548
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131986"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="14443-103">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="14443-103">Create securityBaselineDeviceState</span></span>

<span data-ttu-id="14443-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14443-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14443-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14443-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14443-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14443-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14443-107">创建新的 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14443-107">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14443-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="14443-108">Prerequisites</span></span>
<span data-ttu-id="14443-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14443-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="14443-111">Permission type</span></span>|<span data-ttu-id="14443-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14443-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14443-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14443-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14443-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14443-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14443-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14443-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14443-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14443-116">Not supported.</span></span>|
|<span data-ttu-id="14443-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="14443-117">Application</span></span>|<span data-ttu-id="14443-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14443-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14443-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14443-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="14443-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14443-120">Request headers</span></span>
|<span data-ttu-id="14443-121">标头</span><span class="sxs-lookup"><span data-stu-id="14443-121">Header</span></span>|<span data-ttu-id="14443-122">值</span><span class="sxs-lookup"><span data-stu-id="14443-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14443-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14443-123">Authorization</span></span>|<span data-ttu-id="14443-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14443-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14443-125">接受</span><span class="sxs-lookup"><span data-stu-id="14443-125">Accept</span></span>|<span data-ttu-id="14443-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14443-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14443-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14443-127">Request body</span></span>
<span data-ttu-id="14443-128">在请求正文中，提供 securityBaselineDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14443-128">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="14443-129">下表显示创建 securityBaselineDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="14443-129">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="14443-130">属性</span><span class="sxs-lookup"><span data-stu-id="14443-130">Property</span></span>|<span data-ttu-id="14443-131">类型</span><span class="sxs-lookup"><span data-stu-id="14443-131">Type</span></span>|<span data-ttu-id="14443-132">说明</span><span class="sxs-lookup"><span data-stu-id="14443-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14443-133">id</span><span class="sxs-lookup"><span data-stu-id="14443-133">id</span></span>|<span data-ttu-id="14443-134">String</span><span class="sxs-lookup"><span data-stu-id="14443-134">String</span></span>|<span data-ttu-id="14443-135">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="14443-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="14443-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="14443-136">managedDeviceId</span></span>|<span data-ttu-id="14443-137">String</span><span class="sxs-lookup"><span data-stu-id="14443-137">String</span></span>|<span data-ttu-id="14443-138">Intune 设备 ID</span><span class="sxs-lookup"><span data-stu-id="14443-138">Intune device id</span></span>|
|<span data-ttu-id="14443-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="14443-139">deviceDisplayName</span></span>|<span data-ttu-id="14443-140">String</span><span class="sxs-lookup"><span data-stu-id="14443-140">String</span></span>|<span data-ttu-id="14443-141">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="14443-141">Display name of the device</span></span>|
|<span data-ttu-id="14443-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="14443-142">userPrincipalName</span></span>|<span data-ttu-id="14443-143">String</span><span class="sxs-lookup"><span data-stu-id="14443-143">String</span></span>|<span data-ttu-id="14443-144">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="14443-144">User Principal Name</span></span>|
|<span data-ttu-id="14443-145">state</span><span class="sxs-lookup"><span data-stu-id="14443-145">state</span></span>|[<span data-ttu-id="14443-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="14443-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="14443-147">安全基线合规性状态。</span><span class="sxs-lookup"><span data-stu-id="14443-147">Security baseline compliance state.</span></span> <span data-ttu-id="14443-148">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="14443-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="14443-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="14443-149">lastReportedDateTime</span></span>|<span data-ttu-id="14443-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14443-150">DateTimeOffset</span></span>|<span data-ttu-id="14443-151">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="14443-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="14443-152">响应</span><span class="sxs-lookup"><span data-stu-id="14443-152">Response</span></span>
<span data-ttu-id="14443-153">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14443-153">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14443-154">示例</span><span class="sxs-lookup"><span data-stu-id="14443-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="14443-155">请求</span><span class="sxs-lookup"><span data-stu-id="14443-155">Request</span></span>
<span data-ttu-id="14443-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14443-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14443-157">响应</span><span class="sxs-lookup"><span data-stu-id="14443-157">Response</span></span>
<span data-ttu-id="14443-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14443-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




