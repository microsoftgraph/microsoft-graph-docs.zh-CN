---
title: 创建 deviceManagementPartner
description: 创建新的 deviceManagementPartner 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d07b78207ef28632440588bf8e5349a0c9f36f8a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752544"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="eb6d2-103">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="eb6d2-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="eb6d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb6d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb6d2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb6d2-106">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb6d2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb6d2-107">Prerequisites</span></span>
<span data-ttu-id="eb6d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb6d2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb6d2-110">Permission type</span></span>|<span data-ttu-id="eb6d2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb6d2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb6d2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb6d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb6d2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb6d2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb6d2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb6d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb6d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-115">Not supported.</span></span>|
|<span data-ttu-id="eb6d2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb6d2-116">Application</span></span>|<span data-ttu-id="eb6d2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb6d2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb6d2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb6d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="eb6d2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb6d2-119">Request headers</span></span>
|<span data-ttu-id="eb6d2-120">标头</span><span class="sxs-lookup"><span data-stu-id="eb6d2-120">Header</span></span>|<span data-ttu-id="eb6d2-121">值</span><span class="sxs-lookup"><span data-stu-id="eb6d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb6d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb6d2-122">Authorization</span></span>|<span data-ttu-id="eb6d2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb6d2-124">接受</span><span class="sxs-lookup"><span data-stu-id="eb6d2-124">Accept</span></span>|<span data-ttu-id="eb6d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb6d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb6d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb6d2-126">Request body</span></span>
<span data-ttu-id="eb6d2-127">在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="eb6d2-128">下表显示创建 deviceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="eb6d2-129">属性</span><span class="sxs-lookup"><span data-stu-id="eb6d2-129">Property</span></span>|<span data-ttu-id="eb6d2-130">类型</span><span class="sxs-lookup"><span data-stu-id="eb6d2-130">Type</span></span>|<span data-ttu-id="eb6d2-131">说明</span><span class="sxs-lookup"><span data-stu-id="eb6d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb6d2-132">id</span><span class="sxs-lookup"><span data-stu-id="eb6d2-132">id</span></span>|<span data-ttu-id="eb6d2-133">String</span><span class="sxs-lookup"><span data-stu-id="eb6d2-133">String</span></span>|<span data-ttu-id="eb6d2-134">实体的 ID</span><span class="sxs-lookup"><span data-stu-id="eb6d2-134">Id of the entity</span></span>|
|<span data-ttu-id="eb6d2-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="eb6d2-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="eb6d2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb6d2-136">DateTimeOffset</span></span>|<span data-ttu-id="eb6d2-137">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="eb6d2-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="eb6d2-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="eb6d2-138">partnerState</span></span>|[<span data-ttu-id="eb6d2-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="eb6d2-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="eb6d2-140">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-140">Partner state of this tenant.</span></span> <span data-ttu-id="eb6d2-141">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="eb6d2-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="eb6d2-142">partnerAppType</span></span>|[<span data-ttu-id="eb6d2-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="eb6d2-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="eb6d2-144">合作伙伴应用类型。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-144">Partner App type.</span></span> <span data-ttu-id="eb6d2-145">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="eb6d2-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="eb6d2-146">singleTenantAppId</span></span>|<span data-ttu-id="eb6d2-147">String</span><span class="sxs-lookup"><span data-stu-id="eb6d2-147">String</span></span>|<span data-ttu-id="eb6d2-148">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="eb6d2-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="eb6d2-149">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6d2-149">displayName</span></span>|<span data-ttu-id="eb6d2-150">String</span><span class="sxs-lookup"><span data-stu-id="eb6d2-150">String</span></span>|<span data-ttu-id="eb6d2-151">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="eb6d2-151">Partner display name</span></span>|
|<span data-ttu-id="eb6d2-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="eb6d2-152">isConfigured</span></span>|<span data-ttu-id="eb6d2-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb6d2-153">Boolean</span></span>|<span data-ttu-id="eb6d2-154">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="eb6d2-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="eb6d2-155">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb6d2-155">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="eb6d2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb6d2-156">DateTimeOffset</span></span>|<span data-ttu-id="eb6d2-157">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="eb6d2-157">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="eb6d2-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="eb6d2-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="eb6d2-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb6d2-159">DateTimeOffset</span></span>|<span data-ttu-id="eb6d2-160">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="eb6d2-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="eb6d2-161">响应</span><span class="sxs-lookup"><span data-stu-id="eb6d2-161">Response</span></span>
<span data-ttu-id="eb6d2-162">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-162">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb6d2-163">示例</span><span class="sxs-lookup"><span data-stu-id="eb6d2-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb6d2-164">请求</span><span class="sxs-lookup"><span data-stu-id="eb6d2-164">Request</span></span>
<span data-ttu-id="eb6d2-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb6d2-166">响应</span><span class="sxs-lookup"><span data-stu-id="eb6d2-166">Response</span></span>
<span data-ttu-id="eb6d2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb6d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




