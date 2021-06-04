---
title: 创建 managedDeviceMobileAppConfigurationUserStatus
description: 创建新的 managedDeviceMobileAppConfigurationUserStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edeeb8966cef97cc0d581f0d0d356f79dbe71096
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754208"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="5be2d-103">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="5be2d-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="5be2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5be2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5be2d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5be2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5be2d-106">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5be2d-106">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5be2d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5be2d-107">Prerequisites</span></span>
<span data-ttu-id="5be2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5be2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5be2d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5be2d-110">Permission type</span></span>|<span data-ttu-id="5be2d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5be2d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5be2d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5be2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5be2d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5be2d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5be2d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5be2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5be2d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5be2d-115">Not supported.</span></span>|
|<span data-ttu-id="5be2d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5be2d-116">Application</span></span>|<span data-ttu-id="5be2d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5be2d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5be2d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5be2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5be2d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5be2d-119">Request headers</span></span>
|<span data-ttu-id="5be2d-120">标头</span><span class="sxs-lookup"><span data-stu-id="5be2d-120">Header</span></span>|<span data-ttu-id="5be2d-121">值</span><span class="sxs-lookup"><span data-stu-id="5be2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5be2d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5be2d-122">Authorization</span></span>|<span data-ttu-id="5be2d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5be2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5be2d-124">接受</span><span class="sxs-lookup"><span data-stu-id="5be2d-124">Accept</span></span>|<span data-ttu-id="5be2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5be2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5be2d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5be2d-126">Request body</span></span>
<span data-ttu-id="5be2d-127">在请求正文中，提供 managedDeviceMobileAppConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5be2d-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="5be2d-128">下表显示创建 managedDeviceMobileAppConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5be2d-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="5be2d-129">属性</span><span class="sxs-lookup"><span data-stu-id="5be2d-129">Property</span></span>|<span data-ttu-id="5be2d-130">类型</span><span class="sxs-lookup"><span data-stu-id="5be2d-130">Type</span></span>|<span data-ttu-id="5be2d-131">说明</span><span class="sxs-lookup"><span data-stu-id="5be2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5be2d-132">id</span><span class="sxs-lookup"><span data-stu-id="5be2d-132">id</span></span>|<span data-ttu-id="5be2d-133">String</span><span class="sxs-lookup"><span data-stu-id="5be2d-133">String</span></span>|<span data-ttu-id="5be2d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5be2d-134">Key of the entity.</span></span>|
|<span data-ttu-id="5be2d-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5be2d-135">userDisplayName</span></span>|<span data-ttu-id="5be2d-136">String</span><span class="sxs-lookup"><span data-stu-id="5be2d-136">String</span></span>|<span data-ttu-id="5be2d-137">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="5be2d-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5be2d-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="5be2d-138">devicesCount</span></span>|<span data-ttu-id="5be2d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="5be2d-139">Int32</span></span>|<span data-ttu-id="5be2d-140">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="5be2d-140">Devices count for that user.</span></span>|
|<span data-ttu-id="5be2d-141">status</span><span class="sxs-lookup"><span data-stu-id="5be2d-141">status</span></span>|[<span data-ttu-id="5be2d-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5be2d-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5be2d-143">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5be2d-143">Compliance status of the policy report.</span></span> <span data-ttu-id="5be2d-144">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="5be2d-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5be2d-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5be2d-145">lastReportedDateTime</span></span>|<span data-ttu-id="5be2d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5be2d-146">DateTimeOffset</span></span>|<span data-ttu-id="5be2d-147">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="5be2d-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5be2d-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5be2d-148">userPrincipalName</span></span>|<span data-ttu-id="5be2d-149">String</span><span class="sxs-lookup"><span data-stu-id="5be2d-149">String</span></span>|<span data-ttu-id="5be2d-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="5be2d-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="5be2d-151">响应</span><span class="sxs-lookup"><span data-stu-id="5be2d-151">Response</span></span>
<span data-ttu-id="5be2d-152">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5be2d-152">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5be2d-153">示例</span><span class="sxs-lookup"><span data-stu-id="5be2d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="5be2d-154">请求</span><span class="sxs-lookup"><span data-stu-id="5be2d-154">Request</span></span>
<span data-ttu-id="5be2d-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5be2d-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="5be2d-156">响应</span><span class="sxs-lookup"><span data-stu-id="5be2d-156">Response</span></span>
<span data-ttu-id="5be2d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5be2d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




