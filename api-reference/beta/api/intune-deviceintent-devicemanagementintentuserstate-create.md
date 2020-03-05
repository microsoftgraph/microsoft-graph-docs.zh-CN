---
title: 创建 deviceManagementIntentUserState
description: 创建新的 deviceManagementIntentUserState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57e8c29e9312e105dde36abb28e5bb91afed3d6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470761"
---
# <a name="create-devicemanagementintentuserstate"></a><span data-ttu-id="85929-103">创建 deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="85929-103">Create deviceManagementIntentUserState</span></span>

<span data-ttu-id="85929-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="85929-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85929-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85929-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85929-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85929-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85929-107">创建新的[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="85929-107">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85929-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85929-108">Prerequisites</span></span>
<span data-ttu-id="85929-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85929-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85929-111">Permission type</span></span>|<span data-ttu-id="85929-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85929-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85929-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85929-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85929-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85929-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85929-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85929-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85929-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85929-116">Not supported.</span></span>|
|<span data-ttu-id="85929-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85929-117">Application</span></span>|<span data-ttu-id="85929-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85929-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85929-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85929-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="85929-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85929-120">Request headers</span></span>
|<span data-ttu-id="85929-121">标头</span><span class="sxs-lookup"><span data-stu-id="85929-121">Header</span></span>|<span data-ttu-id="85929-122">值</span><span class="sxs-lookup"><span data-stu-id="85929-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85929-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85929-123">Authorization</span></span>|<span data-ttu-id="85929-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85929-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85929-125">接受</span><span class="sxs-lookup"><span data-stu-id="85929-125">Accept</span></span>|<span data-ttu-id="85929-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85929-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85929-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85929-127">Request body</span></span>
<span data-ttu-id="85929-128">在请求正文中，提供 deviceManagementIntentUserState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85929-128">In the request body, supply a JSON representation for the deviceManagementIntentUserState object.</span></span>

<span data-ttu-id="85929-129">下表显示创建 deviceManagementIntentUserState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85929-129">The following table shows the properties that are required when you create the deviceManagementIntentUserState.</span></span>

|<span data-ttu-id="85929-130">属性</span><span class="sxs-lookup"><span data-stu-id="85929-130">Property</span></span>|<span data-ttu-id="85929-131">类型</span><span class="sxs-lookup"><span data-stu-id="85929-131">Type</span></span>|<span data-ttu-id="85929-132">说明</span><span class="sxs-lookup"><span data-stu-id="85929-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85929-133">id</span><span class="sxs-lookup"><span data-stu-id="85929-133">id</span></span>|<span data-ttu-id="85929-134">String</span><span class="sxs-lookup"><span data-stu-id="85929-134">String</span></span>|<span data-ttu-id="85929-135">ID</span><span class="sxs-lookup"><span data-stu-id="85929-135">The ID</span></span>|
|<span data-ttu-id="85929-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85929-136">userPrincipalName</span></span>|<span data-ttu-id="85929-137">String</span><span class="sxs-lookup"><span data-stu-id="85929-137">String</span></span>|<span data-ttu-id="85929-138">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="85929-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="85929-139">userName</span><span class="sxs-lookup"><span data-stu-id="85929-139">userName</span></span>|<span data-ttu-id="85929-140">String</span><span class="sxs-lookup"><span data-stu-id="85929-140">String</span></span>|<span data-ttu-id="85929-141">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="85929-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="85929-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="85929-142">deviceCount</span></span>|<span data-ttu-id="85929-143">Int32</span><span class="sxs-lookup"><span data-stu-id="85929-143">Int32</span></span>|<span data-ttu-id="85929-144">属于某个意图的用户的设备计数</span><span class="sxs-lookup"><span data-stu-id="85929-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="85929-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="85929-145">lastReportedDateTime</span></span>|<span data-ttu-id="85929-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85929-146">DateTimeOffset</span></span>|<span data-ttu-id="85929-147">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="85929-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="85929-148">state</span><span class="sxs-lookup"><span data-stu-id="85929-148">state</span></span>|[<span data-ttu-id="85929-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="85929-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="85929-150">意图的用户状态。</span><span class="sxs-lookup"><span data-stu-id="85929-150">User state for an intent.</span></span> <span data-ttu-id="85929-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="85929-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="85929-152">响应</span><span class="sxs-lookup"><span data-stu-id="85929-152">Response</span></span>
<span data-ttu-id="85929-153">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="85929-153">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85929-154">示例</span><span class="sxs-lookup"><span data-stu-id="85929-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="85929-155">请求</span><span class="sxs-lookup"><span data-stu-id="85929-155">Request</span></span>
<span data-ttu-id="85929-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85929-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
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

### <a name="response"></a><span data-ttu-id="85929-157">响应</span><span class="sxs-lookup"><span data-stu-id="85929-157">Response</span></span>
<span data-ttu-id="85929-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85929-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





