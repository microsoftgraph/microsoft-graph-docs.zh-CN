---
title: 更新 deviceManagementPartner
description: 更新 deviceManagementPartner 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7997090593748bd64ca7982d98a9595058647871
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149243"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="cf946-103">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="cf946-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="cf946-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf946-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf946-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf946-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf946-106">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cf946-106">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf946-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf946-107">Prerequisites</span></span>
<span data-ttu-id="cf946-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cf946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf946-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf946-110">Permission type</span></span>|<span data-ttu-id="cf946-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf946-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf946-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf946-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf946-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf946-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf946-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf946-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf946-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf946-115">Not supported.</span></span>|
|<span data-ttu-id="cf946-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf946-116">Application</span></span>|<span data-ttu-id="cf946-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf946-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf946-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf946-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="cf946-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf946-119">Request headers</span></span>
|<span data-ttu-id="cf946-120">标头</span><span class="sxs-lookup"><span data-stu-id="cf946-120">Header</span></span>|<span data-ttu-id="cf946-121">值</span><span class="sxs-lookup"><span data-stu-id="cf946-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf946-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf946-122">Authorization</span></span>|<span data-ttu-id="cf946-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf946-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf946-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cf946-124">Accept</span></span>|<span data-ttu-id="cf946-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf946-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf946-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf946-126">Request body</span></span>
<span data-ttu-id="cf946-127">在请求正文中，提供 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf946-127">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="cf946-128">下表显示创建 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cf946-128">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="cf946-129">属性</span><span class="sxs-lookup"><span data-stu-id="cf946-129">Property</span></span>|<span data-ttu-id="cf946-130">类型</span><span class="sxs-lookup"><span data-stu-id="cf946-130">Type</span></span>|<span data-ttu-id="cf946-131">说明</span><span class="sxs-lookup"><span data-stu-id="cf946-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf946-132">id</span><span class="sxs-lookup"><span data-stu-id="cf946-132">id</span></span>|<span data-ttu-id="cf946-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cf946-133">String</span></span>|<span data-ttu-id="cf946-134">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="cf946-134">Id of the entity</span></span>|
|<span data-ttu-id="cf946-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="cf946-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="cf946-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf946-136">DateTimeOffset</span></span>|<span data-ttu-id="cf946-137">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="cf946-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="cf946-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="cf946-138">partnerState</span></span>|[<span data-ttu-id="cf946-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="cf946-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="cf946-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="cf946-140">Partner state of this tenant.</span></span> <span data-ttu-id="cf946-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="cf946-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="cf946-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="cf946-142">partnerAppType</span></span>|[<span data-ttu-id="cf946-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="cf946-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="cf946-144">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="cf946-144">Partner App type.</span></span> <span data-ttu-id="cf946-145">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="cf946-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="cf946-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="cf946-146">singleTenantAppId</span></span>|<span data-ttu-id="cf946-147">String</span><span class="sxs-lookup"><span data-stu-id="cf946-147">String</span></span>|<span data-ttu-id="cf946-148">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="cf946-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="cf946-149">displayName</span><span class="sxs-lookup"><span data-stu-id="cf946-149">displayName</span></span>|<span data-ttu-id="cf946-150">String</span><span class="sxs-lookup"><span data-stu-id="cf946-150">String</span></span>|<span data-ttu-id="cf946-151">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="cf946-151">Partner display name</span></span>|
|<span data-ttu-id="cf946-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="cf946-152">isConfigured</span></span>|<span data-ttu-id="cf946-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf946-153">Boolean</span></span>|<span data-ttu-id="cf946-154">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="cf946-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="cf946-155">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="cf946-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="cf946-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf946-156">DateTimeOffset</span></span>|<span data-ttu-id="cf946-157">将删除 PartnerDevices 时, UTC 格式的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="cf946-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="cf946-158">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="cf946-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="cf946-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="cf946-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="cf946-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf946-160">DateTimeOffset</span></span>|<span data-ttu-id="cf946-161">PartnerDevices 将被标记为不符合时的 UTC 格式的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cf946-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="cf946-162">这将很快变成 obselete。</span><span class="sxs-lookup"><span data-stu-id="cf946-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="cf946-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf946-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="cf946-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf946-164">DateTimeOffset</span></span>|<span data-ttu-id="cf946-165">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="cf946-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="cf946-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="cf946-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="cf946-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf946-167">DateTimeOffset</span></span>|<span data-ttu-id="cf946-168">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="cf946-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="cf946-169">响应</span><span class="sxs-lookup"><span data-stu-id="cf946-169">Response</span></span>
<span data-ttu-id="cf946-170">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf946-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf946-171">示例</span><span class="sxs-lookup"><span data-stu-id="cf946-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf946-172">请求</span><span class="sxs-lookup"><span data-stu-id="cf946-172">Request</span></span>
<span data-ttu-id="cf946-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf946-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="cf946-174">响应</span><span class="sxs-lookup"><span data-stu-id="cf946-174">Response</span></span>
<span data-ttu-id="cf946-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf946-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 713

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```




