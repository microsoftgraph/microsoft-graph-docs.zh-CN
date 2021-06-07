---
title: 更新 deviceManagementPartner
description: 更新 deviceManagementPartner 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ef54e2a53cb9293859ca40043733286dbb59b9d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752537"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="2036a-103">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="2036a-103">Update deviceManagementPartner</span></span>

<span data-ttu-id="2036a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2036a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2036a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2036a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2036a-106">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2036a-106">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2036a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2036a-107">Prerequisites</span></span>
<span data-ttu-id="2036a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2036a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2036a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2036a-110">Permission type</span></span>|<span data-ttu-id="2036a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2036a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2036a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2036a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2036a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2036a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2036a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2036a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2036a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2036a-115">Not supported.</span></span>|
|<span data-ttu-id="2036a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2036a-116">Application</span></span>|<span data-ttu-id="2036a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2036a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2036a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2036a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="2036a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2036a-119">Request headers</span></span>
|<span data-ttu-id="2036a-120">标头</span><span class="sxs-lookup"><span data-stu-id="2036a-120">Header</span></span>|<span data-ttu-id="2036a-121">值</span><span class="sxs-lookup"><span data-stu-id="2036a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2036a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2036a-122">Authorization</span></span>|<span data-ttu-id="2036a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2036a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2036a-124">接受</span><span class="sxs-lookup"><span data-stu-id="2036a-124">Accept</span></span>|<span data-ttu-id="2036a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2036a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2036a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2036a-126">Request body</span></span>
<span data-ttu-id="2036a-127">在请求正文中，提供 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2036a-127">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="2036a-128">下表显示创建 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2036a-128">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="2036a-129">属性</span><span class="sxs-lookup"><span data-stu-id="2036a-129">Property</span></span>|<span data-ttu-id="2036a-130">类型</span><span class="sxs-lookup"><span data-stu-id="2036a-130">Type</span></span>|<span data-ttu-id="2036a-131">说明</span><span class="sxs-lookup"><span data-stu-id="2036a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2036a-132">id</span><span class="sxs-lookup"><span data-stu-id="2036a-132">id</span></span>|<span data-ttu-id="2036a-133">String</span><span class="sxs-lookup"><span data-stu-id="2036a-133">String</span></span>|<span data-ttu-id="2036a-134">实体的 ID</span><span class="sxs-lookup"><span data-stu-id="2036a-134">Id of the entity</span></span>|
|<span data-ttu-id="2036a-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="2036a-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="2036a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2036a-136">DateTimeOffset</span></span>|<span data-ttu-id="2036a-137">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="2036a-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="2036a-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="2036a-138">partnerState</span></span>|[<span data-ttu-id="2036a-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="2036a-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="2036a-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="2036a-140">Partner state of this tenant.</span></span> <span data-ttu-id="2036a-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="2036a-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="2036a-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="2036a-142">partnerAppType</span></span>|[<span data-ttu-id="2036a-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="2036a-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="2036a-144">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="2036a-144">Partner App type.</span></span> <span data-ttu-id="2036a-145">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="2036a-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="2036a-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="2036a-146">singleTenantAppId</span></span>|<span data-ttu-id="2036a-147">String</span><span class="sxs-lookup"><span data-stu-id="2036a-147">String</span></span>|<span data-ttu-id="2036a-148">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="2036a-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="2036a-149">displayName</span><span class="sxs-lookup"><span data-stu-id="2036a-149">displayName</span></span>|<span data-ttu-id="2036a-150">String</span><span class="sxs-lookup"><span data-stu-id="2036a-150">String</span></span>|<span data-ttu-id="2036a-151">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="2036a-151">Partner display name</span></span>|
|<span data-ttu-id="2036a-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="2036a-152">isConfigured</span></span>|<span data-ttu-id="2036a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="2036a-153">Boolean</span></span>|<span data-ttu-id="2036a-154">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="2036a-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="2036a-155">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="2036a-155">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="2036a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2036a-156">DateTimeOffset</span></span>|<span data-ttu-id="2036a-157">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="2036a-157">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="2036a-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="2036a-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="2036a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2036a-159">DateTimeOffset</span></span>|<span data-ttu-id="2036a-160">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="2036a-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="2036a-161">响应</span><span class="sxs-lookup"><span data-stu-id="2036a-161">Response</span></span>
<span data-ttu-id="2036a-162">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2036a-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2036a-163">示例</span><span class="sxs-lookup"><span data-stu-id="2036a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2036a-164">请求</span><span class="sxs-lookup"><span data-stu-id="2036a-164">Request</span></span>
<span data-ttu-id="2036a-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2036a-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2036a-166">响应</span><span class="sxs-lookup"><span data-stu-id="2036a-166">Response</span></span>
<span data-ttu-id="2036a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2036a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```




