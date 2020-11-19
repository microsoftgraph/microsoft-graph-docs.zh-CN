---
title: 更新 deviceManagementIntentUserState
description: 更新 deviceManagementIntentUserState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8986e5e224c63a61e1958e6a86047eaa0e8d235a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213026"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="b0cd7-103">更新 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="b0cd7-103">Update deviceManagementIntentUserState</span></span>

<span data-ttu-id="b0cd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0cd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0cd7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0cd7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0cd7-107">更新 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-107">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0cd7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0cd7-108">Prerequisites</span></span>
<span data-ttu-id="b0cd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0cd7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0cd7-111">Permission type</span></span>|<span data-ttu-id="b0cd7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0cd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0cd7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0cd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0cd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0cd7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0cd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0cd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-116">Not supported.</span></span>|
|<span data-ttu-id="b0cd7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0cd7-117">Application</span></span>|<span data-ttu-id="b0cd7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cd7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0cd7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0cd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b0cd7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0cd7-120">Request headers</span></span>
|<span data-ttu-id="b0cd7-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0cd7-121">Header</span></span>|<span data-ttu-id="b0cd7-122">值</span><span class="sxs-lookup"><span data-stu-id="b0cd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0cd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0cd7-123">Authorization</span></span>|<span data-ttu-id="b0cd7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0cd7-125">接受</span><span class="sxs-lookup"><span data-stu-id="b0cd7-125">Accept</span></span>|<span data-ttu-id="b0cd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0cd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0cd7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0cd7-127">Request body</span></span>
<span data-ttu-id="b0cd7-128">在请求正文中，提供 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="b0cd7-129">下表显示创建 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="b0cd7-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0cd7-130">Property</span></span>|<span data-ttu-id="b0cd7-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0cd7-131">Type</span></span>|<span data-ttu-id="b0cd7-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0cd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0cd7-133">id</span><span class="sxs-lookup"><span data-stu-id="b0cd7-133">id</span></span>|<span data-ttu-id="b0cd7-134">String</span><span class="sxs-lookup"><span data-stu-id="b0cd7-134">String</span></span>|<span data-ttu-id="b0cd7-135">ID</span><span class="sxs-lookup"><span data-stu-id="b0cd7-135">The ID</span></span>|
|<span data-ttu-id="b0cd7-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0cd7-136">userPrincipalName</span></span>|<span data-ttu-id="b0cd7-137">String</span><span class="sxs-lookup"><span data-stu-id="b0cd7-137">String</span></span>|<span data-ttu-id="b0cd7-138">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b0cd7-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="b0cd7-139">userName</span><span class="sxs-lookup"><span data-stu-id="b0cd7-139">userName</span></span>|<span data-ttu-id="b0cd7-140">String</span><span class="sxs-lookup"><span data-stu-id="b0cd7-140">String</span></span>|<span data-ttu-id="b0cd7-141">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="b0cd7-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="b0cd7-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b0cd7-142">deviceCount</span></span>|<span data-ttu-id="b0cd7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b0cd7-143">Int32</span></span>|<span data-ttu-id="b0cd7-144">属于某个意图的用户的设备计数</span><span class="sxs-lookup"><span data-stu-id="b0cd7-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="b0cd7-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0cd7-145">lastReportedDateTime</span></span>|<span data-ttu-id="b0cd7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0cd7-146">DateTimeOffset</span></span>|<span data-ttu-id="b0cd7-147">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="b0cd7-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="b0cd7-148">state</span><span class="sxs-lookup"><span data-stu-id="b0cd7-148">state</span></span>|[<span data-ttu-id="b0cd7-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b0cd7-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b0cd7-150">意图的用户状态。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-150">User state for an intent.</span></span> <span data-ttu-id="b0cd7-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="b0cd7-152">响应</span><span class="sxs-lookup"><span data-stu-id="b0cd7-152">Response</span></span>
<span data-ttu-id="b0cd7-153">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0cd7-154">示例</span><span class="sxs-lookup"><span data-stu-id="b0cd7-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0cd7-155">请求</span><span class="sxs-lookup"><span data-stu-id="b0cd7-155">Request</span></span>
<span data-ttu-id="b0cd7-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0cd7-157">响应</span><span class="sxs-lookup"><span data-stu-id="b0cd7-157">Response</span></span>
<span data-ttu-id="b0cd7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0cd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




