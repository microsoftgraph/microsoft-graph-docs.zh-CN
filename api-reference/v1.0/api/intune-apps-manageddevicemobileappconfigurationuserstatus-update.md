---
title: 更新 managedDeviceMobileAppConfigurationUserStatus
description: 更新 managedDeviceMobileAppConfigurationUserStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b1b0cfab88b44adaaa95b2b519ce5cc34c94d5b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754201"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="1684b-103">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="1684b-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="1684b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1684b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1684b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1684b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1684b-106">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1684b-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1684b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1684b-107">Prerequisites</span></span>
<span data-ttu-id="1684b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1684b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1684b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1684b-110">Permission type</span></span>|<span data-ttu-id="1684b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1684b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1684b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1684b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1684b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1684b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1684b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1684b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1684b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1684b-115">Not supported.</span></span>|
|<span data-ttu-id="1684b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1684b-116">Application</span></span>|<span data-ttu-id="1684b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1684b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1684b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1684b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1684b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1684b-119">Request headers</span></span>
|<span data-ttu-id="1684b-120">标头</span><span class="sxs-lookup"><span data-stu-id="1684b-120">Header</span></span>|<span data-ttu-id="1684b-121">值</span><span class="sxs-lookup"><span data-stu-id="1684b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1684b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1684b-122">Authorization</span></span>|<span data-ttu-id="1684b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1684b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1684b-124">接受</span><span class="sxs-lookup"><span data-stu-id="1684b-124">Accept</span></span>|<span data-ttu-id="1684b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1684b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1684b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1684b-126">Request body</span></span>
<span data-ttu-id="1684b-127">在请求正文中，提供 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1684b-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="1684b-128">下表显示创建 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1684b-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="1684b-129">属性</span><span class="sxs-lookup"><span data-stu-id="1684b-129">Property</span></span>|<span data-ttu-id="1684b-130">类型</span><span class="sxs-lookup"><span data-stu-id="1684b-130">Type</span></span>|<span data-ttu-id="1684b-131">说明</span><span class="sxs-lookup"><span data-stu-id="1684b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1684b-132">id</span><span class="sxs-lookup"><span data-stu-id="1684b-132">id</span></span>|<span data-ttu-id="1684b-133">String</span><span class="sxs-lookup"><span data-stu-id="1684b-133">String</span></span>|<span data-ttu-id="1684b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1684b-134">Key of the entity.</span></span>|
|<span data-ttu-id="1684b-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1684b-135">userDisplayName</span></span>|<span data-ttu-id="1684b-136">String</span><span class="sxs-lookup"><span data-stu-id="1684b-136">String</span></span>|<span data-ttu-id="1684b-137">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="1684b-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1684b-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="1684b-138">devicesCount</span></span>|<span data-ttu-id="1684b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1684b-139">Int32</span></span>|<span data-ttu-id="1684b-140">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="1684b-140">Devices count for that user.</span></span>|
|<span data-ttu-id="1684b-141">status</span><span class="sxs-lookup"><span data-stu-id="1684b-141">status</span></span>|[<span data-ttu-id="1684b-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1684b-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1684b-143">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="1684b-143">Compliance status of the policy report.</span></span> <span data-ttu-id="1684b-144">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="1684b-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1684b-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1684b-145">lastReportedDateTime</span></span>|<span data-ttu-id="1684b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1684b-146">DateTimeOffset</span></span>|<span data-ttu-id="1684b-147">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="1684b-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1684b-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1684b-148">userPrincipalName</span></span>|<span data-ttu-id="1684b-149">String</span><span class="sxs-lookup"><span data-stu-id="1684b-149">String</span></span>|<span data-ttu-id="1684b-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="1684b-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1684b-151">响应</span><span class="sxs-lookup"><span data-stu-id="1684b-151">Response</span></span>
<span data-ttu-id="1684b-152">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1684b-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1684b-153">示例</span><span class="sxs-lookup"><span data-stu-id="1684b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1684b-154">请求</span><span class="sxs-lookup"><span data-stu-id="1684b-154">Request</span></span>
<span data-ttu-id="1684b-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1684b-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="1684b-156">响应</span><span class="sxs-lookup"><span data-stu-id="1684b-156">Response</span></span>
<span data-ttu-id="1684b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1684b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




