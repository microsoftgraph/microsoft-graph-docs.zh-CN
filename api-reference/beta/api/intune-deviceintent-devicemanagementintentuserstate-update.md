---
title: 更新 deviceManagementIntentUserState
description: 更新 deviceManagementIntentUserState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 223a10e2a46f650e3d390611380bf6c74073b560
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132007"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="f803d-103">更新 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="f803d-103">Update deviceManagementIntentUserState</span></span>

<span data-ttu-id="f803d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f803d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f803d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f803d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f803d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f803d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f803d-107">更新 [deviceManagementIntentUserState 对象](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f803d-107">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f803d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f803d-108">Prerequisites</span></span>
<span data-ttu-id="f803d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f803d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f803d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f803d-111">Permission type</span></span>|<span data-ttu-id="f803d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f803d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f803d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f803d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f803d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f803d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f803d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f803d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f803d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f803d-116">Not supported.</span></span>|
|<span data-ttu-id="f803d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f803d-117">Application</span></span>|<span data-ttu-id="f803d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f803d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f803d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f803d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f803d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f803d-120">Request headers</span></span>
|<span data-ttu-id="f803d-121">标头</span><span class="sxs-lookup"><span data-stu-id="f803d-121">Header</span></span>|<span data-ttu-id="f803d-122">值</span><span class="sxs-lookup"><span data-stu-id="f803d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f803d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f803d-123">Authorization</span></span>|<span data-ttu-id="f803d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f803d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f803d-125">接受</span><span class="sxs-lookup"><span data-stu-id="f803d-125">Accept</span></span>|<span data-ttu-id="f803d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f803d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f803d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f803d-127">Request body</span></span>
<span data-ttu-id="f803d-128">在请求正文中，提供 [deviceManagementIntentUserState 对象的](../resources/intune-deviceintent-devicemanagementintentuserstate.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f803d-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="f803d-129">下表显示创建 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f803d-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="f803d-130">属性</span><span class="sxs-lookup"><span data-stu-id="f803d-130">Property</span></span>|<span data-ttu-id="f803d-131">类型</span><span class="sxs-lookup"><span data-stu-id="f803d-131">Type</span></span>|<span data-ttu-id="f803d-132">说明</span><span class="sxs-lookup"><span data-stu-id="f803d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f803d-133">id</span><span class="sxs-lookup"><span data-stu-id="f803d-133">id</span></span>|<span data-ttu-id="f803d-134">String</span><span class="sxs-lookup"><span data-stu-id="f803d-134">String</span></span>|<span data-ttu-id="f803d-135">The ID</span><span class="sxs-lookup"><span data-stu-id="f803d-135">The ID</span></span>|
|<span data-ttu-id="f803d-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f803d-136">userPrincipalName</span></span>|<span data-ttu-id="f803d-137">String</span><span class="sxs-lookup"><span data-stu-id="f803d-137">String</span></span>|<span data-ttu-id="f803d-138">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f803d-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="f803d-139">userName</span><span class="sxs-lookup"><span data-stu-id="f803d-139">userName</span></span>|<span data-ttu-id="f803d-140">String</span><span class="sxs-lookup"><span data-stu-id="f803d-140">String</span></span>|<span data-ttu-id="f803d-141">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="f803d-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="f803d-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f803d-142">deviceCount</span></span>|<span data-ttu-id="f803d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f803d-143">Int32</span></span>|<span data-ttu-id="f803d-144">出于意图而属于用户的设备的计数</span><span class="sxs-lookup"><span data-stu-id="f803d-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="f803d-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f803d-145">lastReportedDateTime</span></span>|<span data-ttu-id="f803d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f803d-146">DateTimeOffset</span></span>|<span data-ttu-id="f803d-147">意图报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="f803d-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="f803d-148">state</span><span class="sxs-lookup"><span data-stu-id="f803d-148">state</span></span>|[<span data-ttu-id="f803d-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f803d-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f803d-150">意图的用户状态。</span><span class="sxs-lookup"><span data-stu-id="f803d-150">User state for an intent.</span></span> <span data-ttu-id="f803d-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f803d-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="f803d-152">响应</span><span class="sxs-lookup"><span data-stu-id="f803d-152">Response</span></span>
<span data-ttu-id="f803d-153">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f803d-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f803d-154">示例</span><span class="sxs-lookup"><span data-stu-id="f803d-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="f803d-155">请求</span><span class="sxs-lookup"><span data-stu-id="f803d-155">Request</span></span>
<span data-ttu-id="f803d-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f803d-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```

### <a name="response"></a><span data-ttu-id="f803d-157">响应</span><span class="sxs-lookup"><span data-stu-id="f803d-157">Response</span></span>
<span data-ttu-id="f803d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f803d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "0201286a-286a-0201-6a28-01026a280102",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```




