---
title: 更新 deviceManagementIntentUserState
description: 更新 deviceManagementIntentUserState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa492e9b758e95c80fae589e70fea823b4ac98f8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325767"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="78696-103">更新 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="78696-103">Update deviceManagementIntentUserState</span></span>

<span data-ttu-id="78696-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78696-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78696-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78696-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78696-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78696-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78696-107">更新[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="78696-107">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78696-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="78696-108">Prerequisites</span></span>
<span data-ttu-id="78696-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78696-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="78696-111">Permission type</span></span>|<span data-ttu-id="78696-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78696-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78696-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78696-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78696-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78696-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78696-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78696-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78696-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="78696-116">Not supported.</span></span>|
|<span data-ttu-id="78696-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="78696-117">Application</span></span>|<span data-ttu-id="78696-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78696-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78696-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78696-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="78696-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="78696-120">Request headers</span></span>
|<span data-ttu-id="78696-121">标头</span><span class="sxs-lookup"><span data-stu-id="78696-121">Header</span></span>|<span data-ttu-id="78696-122">值</span><span class="sxs-lookup"><span data-stu-id="78696-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78696-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78696-123">Authorization</span></span>|<span data-ttu-id="78696-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78696-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78696-125">接受</span><span class="sxs-lookup"><span data-stu-id="78696-125">Accept</span></span>|<span data-ttu-id="78696-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78696-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78696-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="78696-127">Request body</span></span>
<span data-ttu-id="78696-128">在请求正文中，提供[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78696-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="78696-129">下表显示创建[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78696-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="78696-130">属性</span><span class="sxs-lookup"><span data-stu-id="78696-130">Property</span></span>|<span data-ttu-id="78696-131">类型</span><span class="sxs-lookup"><span data-stu-id="78696-131">Type</span></span>|<span data-ttu-id="78696-132">说明</span><span class="sxs-lookup"><span data-stu-id="78696-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78696-133">id</span><span class="sxs-lookup"><span data-stu-id="78696-133">id</span></span>|<span data-ttu-id="78696-134">String</span><span class="sxs-lookup"><span data-stu-id="78696-134">String</span></span>|<span data-ttu-id="78696-135">ID</span><span class="sxs-lookup"><span data-stu-id="78696-135">The ID</span></span>|
|<span data-ttu-id="78696-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78696-136">userPrincipalName</span></span>|<span data-ttu-id="78696-137">字符串</span><span class="sxs-lookup"><span data-stu-id="78696-137">String</span></span>|<span data-ttu-id="78696-138">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="78696-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="78696-139">userName</span><span class="sxs-lookup"><span data-stu-id="78696-139">userName</span></span>|<span data-ttu-id="78696-140">String</span><span class="sxs-lookup"><span data-stu-id="78696-140">String</span></span>|<span data-ttu-id="78696-141">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="78696-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="78696-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="78696-142">deviceCount</span></span>|<span data-ttu-id="78696-143">Int32</span><span class="sxs-lookup"><span data-stu-id="78696-143">Int32</span></span>|<span data-ttu-id="78696-144">属于某个意图的用户的设备计数</span><span class="sxs-lookup"><span data-stu-id="78696-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="78696-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="78696-145">lastReportedDateTime</span></span>|<span data-ttu-id="78696-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78696-146">DateTimeOffset</span></span>|<span data-ttu-id="78696-147">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="78696-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="78696-148">state</span><span class="sxs-lookup"><span data-stu-id="78696-148">state</span></span>|[<span data-ttu-id="78696-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="78696-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="78696-150">意图的用户状态。</span><span class="sxs-lookup"><span data-stu-id="78696-150">User state for an intent.</span></span> <span data-ttu-id="78696-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="78696-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="78696-152">响应</span><span class="sxs-lookup"><span data-stu-id="78696-152">Response</span></span>
<span data-ttu-id="78696-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="78696-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78696-154">示例</span><span class="sxs-lookup"><span data-stu-id="78696-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="78696-155">请求</span><span class="sxs-lookup"><span data-stu-id="78696-155">Request</span></span>
<span data-ttu-id="78696-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78696-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78696-157">响应</span><span class="sxs-lookup"><span data-stu-id="78696-157">Response</span></span>
<span data-ttu-id="78696-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78696-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



