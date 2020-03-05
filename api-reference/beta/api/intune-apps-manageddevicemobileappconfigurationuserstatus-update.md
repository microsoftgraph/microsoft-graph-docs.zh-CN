---
title: 更新 managedDeviceMobileAppConfigurationUserStatus
description: 更新 managedDeviceMobileAppConfigurationUserStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 485c0d5b9fb2ae9a61c66a588bb3a936e833adb4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450977"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="3e18c-103">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="3e18c-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="3e18c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3e18c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e18c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e18c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e18c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e18c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e18c-107">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3e18c-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e18c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3e18c-108">Prerequisites</span></span>
<span data-ttu-id="3e18c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e18c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e18c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e18c-111">Permission type</span></span>|<span data-ttu-id="3e18c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3e18c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e18c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e18c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e18c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e18c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3e18c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e18c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e18c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e18c-116">Not supported.</span></span>|
|<span data-ttu-id="3e18c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e18c-117">Application</span></span>|<span data-ttu-id="3e18c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e18c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e18c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e18c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="3e18c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e18c-120">Request headers</span></span>
|<span data-ttu-id="3e18c-121">标头</span><span class="sxs-lookup"><span data-stu-id="3e18c-121">Header</span></span>|<span data-ttu-id="3e18c-122">值</span><span class="sxs-lookup"><span data-stu-id="3e18c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e18c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e18c-123">Authorization</span></span>|<span data-ttu-id="3e18c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3e18c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e18c-125">接受</span><span class="sxs-lookup"><span data-stu-id="3e18c-125">Accept</span></span>|<span data-ttu-id="3e18c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e18c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e18c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e18c-127">Request body</span></span>
<span data-ttu-id="3e18c-128">在请求正文中，提供 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e18c-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="3e18c-129">下表显示创建 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3e18c-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="3e18c-130">属性</span><span class="sxs-lookup"><span data-stu-id="3e18c-130">Property</span></span>|<span data-ttu-id="3e18c-131">类型</span><span class="sxs-lookup"><span data-stu-id="3e18c-131">Type</span></span>|<span data-ttu-id="3e18c-132">说明</span><span class="sxs-lookup"><span data-stu-id="3e18c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e18c-133">id</span><span class="sxs-lookup"><span data-stu-id="3e18c-133">id</span></span>|<span data-ttu-id="3e18c-134">String</span><span class="sxs-lookup"><span data-stu-id="3e18c-134">String</span></span>|<span data-ttu-id="3e18c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3e18c-135">Key of the entity.</span></span>|
|<span data-ttu-id="3e18c-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e18c-136">userDisplayName</span></span>|<span data-ttu-id="3e18c-137">String</span><span class="sxs-lookup"><span data-stu-id="3e18c-137">String</span></span>|<span data-ttu-id="3e18c-138">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="3e18c-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="3e18c-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="3e18c-139">devicesCount</span></span>|<span data-ttu-id="3e18c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3e18c-140">Int32</span></span>|<span data-ttu-id="3e18c-141">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e18c-141">Devices count for that user.</span></span>|
|<span data-ttu-id="3e18c-142">status</span><span class="sxs-lookup"><span data-stu-id="3e18c-142">status</span></span>|[<span data-ttu-id="3e18c-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3e18c-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3e18c-144">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="3e18c-144">Compliance status of the policy report.</span></span> <span data-ttu-id="3e18c-145">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="3e18c-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3e18c-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e18c-146">lastReportedDateTime</span></span>|<span data-ttu-id="3e18c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e18c-147">DateTimeOffset</span></span>|<span data-ttu-id="3e18c-148">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="3e18c-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="3e18c-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3e18c-149">userPrincipalName</span></span>|<span data-ttu-id="3e18c-150">字符串</span><span class="sxs-lookup"><span data-stu-id="3e18c-150">String</span></span>|<span data-ttu-id="3e18c-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="3e18c-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="3e18c-152">响应</span><span class="sxs-lookup"><span data-stu-id="3e18c-152">Response</span></span>
<span data-ttu-id="3e18c-153">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e18c-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e18c-154">示例</span><span class="sxs-lookup"><span data-stu-id="3e18c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e18c-155">请求</span><span class="sxs-lookup"><span data-stu-id="3e18c-155">Request</span></span>
<span data-ttu-id="3e18c-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e18c-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="3e18c-157">响应</span><span class="sxs-lookup"><span data-stu-id="3e18c-157">Response</span></span>
<span data-ttu-id="3e18c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e18c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





