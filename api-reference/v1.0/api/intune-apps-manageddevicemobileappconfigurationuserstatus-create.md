---
title: 创建 managedDeviceMobileAppConfigurationUserStatus
description: 创建新的 managedDeviceMobileAppConfigurationUserStatus 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da46008eee715c7ecff2057015cb0dacb37102b7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251445"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="fc2b8-103">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="fc2b8-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="fc2b8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2b8-105">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc2b8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc2b8-106">Prerequisites</span></span>
<span data-ttu-id="fc2b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fc2b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc2b8-109">Permission type</span></span>|<span data-ttu-id="fc2b8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc2b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc2b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc2b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc2b8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc2b8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc2b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc2b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc2b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-114">Not supported.</span></span>|
|<span data-ttu-id="fc2b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc2b8-115">Application</span></span>|<span data-ttu-id="fc2b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc2b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc2b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fc2b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc2b8-118">Request headers</span></span>
|<span data-ttu-id="fc2b8-119">标头</span><span class="sxs-lookup"><span data-stu-id="fc2b8-119">Header</span></span>|<span data-ttu-id="fc2b8-120">值</span><span class="sxs-lookup"><span data-stu-id="fc2b8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc2b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc2b8-121">Authorization</span></span>|<span data-ttu-id="fc2b8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc2b8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fc2b8-123">Accept</span></span>|<span data-ttu-id="fc2b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc2b8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc2b8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc2b8-125">Request body</span></span>
<span data-ttu-id="fc2b8-126">在请求正文中，提供 managedDeviceMobileAppConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="fc2b8-127">下表显示创建 managedDeviceMobileAppConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="fc2b8-128">属性</span><span class="sxs-lookup"><span data-stu-id="fc2b8-128">Property</span></span>|<span data-ttu-id="fc2b8-129">类型</span><span class="sxs-lookup"><span data-stu-id="fc2b8-129">Type</span></span>|<span data-ttu-id="fc2b8-130">说明</span><span class="sxs-lookup"><span data-stu-id="fc2b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2b8-131">id</span><span class="sxs-lookup"><span data-stu-id="fc2b8-131">id</span></span>|<span data-ttu-id="fc2b8-132">字符串</span><span class="sxs-lookup"><span data-stu-id="fc2b8-132">String</span></span>|<span data-ttu-id="fc2b8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-133">Key of the entity.</span></span>|
|<span data-ttu-id="fc2b8-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fc2b8-134">userDisplayName</span></span>|<span data-ttu-id="fc2b8-135">String</span><span class="sxs-lookup"><span data-stu-id="fc2b8-135">String</span></span>|<span data-ttu-id="fc2b8-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="fc2b8-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="fc2b8-137">devicesCount</span></span>|<span data-ttu-id="fc2b8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2b8-138">Int32</span></span>|<span data-ttu-id="fc2b8-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-139">Devices count for that user.</span></span>|
|<span data-ttu-id="fc2b8-140">status</span><span class="sxs-lookup"><span data-stu-id="fc2b8-140">status</span></span>|[<span data-ttu-id="fc2b8-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fc2b8-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fc2b8-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-142">Compliance status of the policy report.</span></span> <span data-ttu-id="fc2b8-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fc2b8-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc2b8-144">lastReportedDateTime</span></span>|<span data-ttu-id="fc2b8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc2b8-145">DateTimeOffset</span></span>|<span data-ttu-id="fc2b8-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="fc2b8-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc2b8-147">userPrincipalName</span></span>|<span data-ttu-id="fc2b8-148">字符串</span><span class="sxs-lookup"><span data-stu-id="fc2b8-148">String</span></span>|<span data-ttu-id="fc2b8-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="fc2b8-150">响应</span><span class="sxs-lookup"><span data-stu-id="fc2b8-150">Response</span></span>
<span data-ttu-id="fc2b8-151">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc2b8-152">示例</span><span class="sxs-lookup"><span data-stu-id="fc2b8-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc2b8-153">请求</span><span class="sxs-lookup"><span data-stu-id="fc2b8-153">Request</span></span>
<span data-ttu-id="fc2b8-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc2b8-155">响应</span><span class="sxs-lookup"><span data-stu-id="fc2b8-155">Response</span></span>
<span data-ttu-id="fc2b8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc2b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



