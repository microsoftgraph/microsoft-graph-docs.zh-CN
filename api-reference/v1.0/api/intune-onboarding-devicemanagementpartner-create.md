---
title: 创建 deviceManagementPartner
description: 创建新的 deviceManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73df635a4af3acbb55be7ecd1163555ac4f701bc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473202"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="1cec0-103">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1cec0-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="1cec0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cec0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cec0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cec0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cec0-106">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1cec0-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cec0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1cec0-107">Prerequisites</span></span>
<span data-ttu-id="1cec0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cec0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cec0-110">Permission type</span></span>|<span data-ttu-id="1cec0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1cec0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cec0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cec0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cec0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cec0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1cec0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cec0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cec0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cec0-115">Not supported.</span></span>|
|<span data-ttu-id="1cec0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cec0-116">Application</span></span>|<span data-ttu-id="1cec0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cec0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cec0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cec0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="1cec0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cec0-119">Request headers</span></span>
|<span data-ttu-id="1cec0-120">标头</span><span class="sxs-lookup"><span data-stu-id="1cec0-120">Header</span></span>|<span data-ttu-id="1cec0-121">值</span><span class="sxs-lookup"><span data-stu-id="1cec0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cec0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cec0-122">Authorization</span></span>|<span data-ttu-id="1cec0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1cec0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cec0-124">接受</span><span class="sxs-lookup"><span data-stu-id="1cec0-124">Accept</span></span>|<span data-ttu-id="1cec0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cec0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cec0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cec0-126">Request body</span></span>
<span data-ttu-id="1cec0-127">在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cec0-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="1cec0-128">下表显示创建 deviceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1cec0-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="1cec0-129">属性</span><span class="sxs-lookup"><span data-stu-id="1cec0-129">Property</span></span>|<span data-ttu-id="1cec0-130">类型</span><span class="sxs-lookup"><span data-stu-id="1cec0-130">Type</span></span>|<span data-ttu-id="1cec0-131">说明</span><span class="sxs-lookup"><span data-stu-id="1cec0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cec0-132">id</span><span class="sxs-lookup"><span data-stu-id="1cec0-132">id</span></span>|<span data-ttu-id="1cec0-133">String</span><span class="sxs-lookup"><span data-stu-id="1cec0-133">String</span></span>|<span data-ttu-id="1cec0-134">实体的 Id</span><span class="sxs-lookup"><span data-stu-id="1cec0-134">Id of the entity</span></span>|
|<span data-ttu-id="1cec0-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="1cec0-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="1cec0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cec0-136">DateTimeOffset</span></span>|<span data-ttu-id="1cec0-137">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="1cec0-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="1cec0-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="1cec0-138">partnerState</span></span>|[<span data-ttu-id="1cec0-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="1cec0-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="1cec0-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="1cec0-140">Partner state of this tenant.</span></span> <span data-ttu-id="1cec0-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="1cec0-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="1cec0-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="1cec0-142">partnerAppType</span></span>|[<span data-ttu-id="1cec0-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="1cec0-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="1cec0-144">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="1cec0-144">Partner App type.</span></span> <span data-ttu-id="1cec0-145">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="1cec0-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="1cec0-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="1cec0-146">singleTenantAppId</span></span>|<span data-ttu-id="1cec0-147">String</span><span class="sxs-lookup"><span data-stu-id="1cec0-147">String</span></span>|<span data-ttu-id="1cec0-148">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="1cec0-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="1cec0-149">displayName</span><span class="sxs-lookup"><span data-stu-id="1cec0-149">displayName</span></span>|<span data-ttu-id="1cec0-150">String</span><span class="sxs-lookup"><span data-stu-id="1cec0-150">String</span></span>|<span data-ttu-id="1cec0-151">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="1cec0-151">Partner display name</span></span>|
|<span data-ttu-id="1cec0-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="1cec0-152">isConfigured</span></span>|<span data-ttu-id="1cec0-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cec0-153">Boolean</span></span>|<span data-ttu-id="1cec0-154">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="1cec0-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="1cec0-155">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cec0-155">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="1cec0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cec0-156">DateTimeOffset</span></span>|<span data-ttu-id="1cec0-157">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="1cec0-157">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="1cec0-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="1cec0-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="1cec0-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cec0-159">DateTimeOffset</span></span>|<span data-ttu-id="1cec0-160">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="1cec0-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="1cec0-161">响应</span><span class="sxs-lookup"><span data-stu-id="1cec0-161">Response</span></span>
<span data-ttu-id="1cec0-162">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1cec0-162">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cec0-163">示例</span><span class="sxs-lookup"><span data-stu-id="1cec0-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cec0-164">请求</span><span class="sxs-lookup"><span data-stu-id="1cec0-164">Request</span></span>
<span data-ttu-id="1cec0-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1cec0-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="1cec0-166">响应</span><span class="sxs-lookup"><span data-stu-id="1cec0-166">Response</span></span>
<span data-ttu-id="1cec0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1cec0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






