---
title: 创建 deviceConfigurationUserStatus
description: 创建新的 deviceConfigurationUserStatus 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fd000c188158ce9442712959555332340b6da76
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017496"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="dbe24-103">创建 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="dbe24-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="dbe24-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbe24-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbe24-105">创建新的 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbe24-105">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbe24-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="dbe24-106">Prerequisites</span></span>
<span data-ttu-id="dbe24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbe24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe24-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbe24-109">Permission type</span></span>|<span data-ttu-id="dbe24-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dbe24-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbe24-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dbe24-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe24-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dbe24-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbe24-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbe24-114">Not supported.</span></span>|
|<span data-ttu-id="dbe24-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbe24-115">Application</span></span>|<span data-ttu-id="dbe24-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbe24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbe24-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbe24-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="dbe24-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbe24-118">Request headers</span></span>
|<span data-ttu-id="dbe24-119">标头</span><span class="sxs-lookup"><span data-stu-id="dbe24-119">Header</span></span>|<span data-ttu-id="dbe24-120">值</span><span class="sxs-lookup"><span data-stu-id="dbe24-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbe24-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbe24-121">Authorization</span></span>|<span data-ttu-id="dbe24-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dbe24-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbe24-123">接受</span><span class="sxs-lookup"><span data-stu-id="dbe24-123">Accept</span></span>|<span data-ttu-id="dbe24-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dbe24-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbe24-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbe24-125">Request body</span></span>
<span data-ttu-id="dbe24-126">在请求正文中，提供 deviceConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbe24-126">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="dbe24-127">下表显示创建 deviceConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dbe24-127">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="dbe24-128">属性</span><span class="sxs-lookup"><span data-stu-id="dbe24-128">Property</span></span>|<span data-ttu-id="dbe24-129">类型</span><span class="sxs-lookup"><span data-stu-id="dbe24-129">Type</span></span>|<span data-ttu-id="dbe24-130">说明</span><span class="sxs-lookup"><span data-stu-id="dbe24-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe24-131">id</span><span class="sxs-lookup"><span data-stu-id="dbe24-131">id</span></span>|<span data-ttu-id="dbe24-132">String</span><span class="sxs-lookup"><span data-stu-id="dbe24-132">String</span></span>|<span data-ttu-id="dbe24-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dbe24-133">Key of the entity.</span></span>|
|<span data-ttu-id="dbe24-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dbe24-134">userDisplayName</span></span>|<span data-ttu-id="dbe24-135">String</span><span class="sxs-lookup"><span data-stu-id="dbe24-135">String</span></span>|<span data-ttu-id="dbe24-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="dbe24-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="dbe24-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="dbe24-137">devicesCount</span></span>|<span data-ttu-id="dbe24-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dbe24-138">Int32</span></span>|<span data-ttu-id="dbe24-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="dbe24-139">Devices count for that user.</span></span>|
|<span data-ttu-id="dbe24-140">status</span><span class="sxs-lookup"><span data-stu-id="dbe24-140">status</span></span>|[<span data-ttu-id="dbe24-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dbe24-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dbe24-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="dbe24-142">Compliance status of the policy report.</span></span> <span data-ttu-id="dbe24-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="dbe24-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dbe24-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbe24-144">lastReportedDateTime</span></span>|<span data-ttu-id="dbe24-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbe24-145">DateTimeOffset</span></span>|<span data-ttu-id="dbe24-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="dbe24-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="dbe24-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dbe24-147">userPrincipalName</span></span>|<span data-ttu-id="dbe24-148">字符串</span><span class="sxs-lookup"><span data-stu-id="dbe24-148">String</span></span>|<span data-ttu-id="dbe24-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="dbe24-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="dbe24-150">响应</span><span class="sxs-lookup"><span data-stu-id="dbe24-150">Response</span></span>
<span data-ttu-id="dbe24-151">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbe24-151">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe24-152">示例</span><span class="sxs-lookup"><span data-stu-id="dbe24-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbe24-153">请求</span><span class="sxs-lookup"><span data-stu-id="dbe24-153">Request</span></span>
<span data-ttu-id="dbe24-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbe24-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="dbe24-155">响应</span><span class="sxs-lookup"><span data-stu-id="dbe24-155">Response</span></span>
<span data-ttu-id="dbe24-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbe24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



