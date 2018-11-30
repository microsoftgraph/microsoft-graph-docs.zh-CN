---
title: 创建 deviceManagementPartner
description: 创建新的 deviceManagementPartner 对象。
ms.openlocfilehash: 038bfecf443972921c7aeacc508e9b1b81331cf4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010781"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="e60ce-103">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e60ce-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="e60ce-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e60ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e60ce-105">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e60ce-105">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e60ce-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e60ce-106">Prerequisites</span></span>
<span data-ttu-id="e60ce-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e60ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e60ce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e60ce-109">Permission type</span></span>|<span data-ttu-id="e60ce-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e60ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e60ce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e60ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e60ce-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e60ce-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e60ce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e60ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e60ce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e60ce-114">Not supported.</span></span>|
|<span data-ttu-id="e60ce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e60ce-115">Application</span></span>|<span data-ttu-id="e60ce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e60ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e60ce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e60ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e60ce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e60ce-118">Request headers</span></span>
|<span data-ttu-id="e60ce-119">标头</span><span class="sxs-lookup"><span data-stu-id="e60ce-119">Header</span></span>|<span data-ttu-id="e60ce-120">值</span><span class="sxs-lookup"><span data-stu-id="e60ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e60ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e60ce-121">Authorization</span></span>|<span data-ttu-id="e60ce-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e60ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e60ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e60ce-123">Accept</span></span>|<span data-ttu-id="e60ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e60ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e60ce-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e60ce-125">Request body</span></span>
<span data-ttu-id="e60ce-126">在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e60ce-126">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="e60ce-127">下表显示创建 deviceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e60ce-127">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="e60ce-128">属性</span><span class="sxs-lookup"><span data-stu-id="e60ce-128">Property</span></span>|<span data-ttu-id="e60ce-129">类型</span><span class="sxs-lookup"><span data-stu-id="e60ce-129">Type</span></span>|<span data-ttu-id="e60ce-130">说明</span><span class="sxs-lookup"><span data-stu-id="e60ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e60ce-131">id</span><span class="sxs-lookup"><span data-stu-id="e60ce-131">id</span></span>|<span data-ttu-id="e60ce-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e60ce-132">String</span></span>|<span data-ttu-id="e60ce-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e60ce-133">Not yet documented</span></span>|
|<span data-ttu-id="e60ce-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="e60ce-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="e60ce-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e60ce-135">DateTimeOffset</span></span>|<span data-ttu-id="e60ce-136">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="e60ce-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="e60ce-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="e60ce-137">partnerState</span></span>|[<span data-ttu-id="e60ce-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="e60ce-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="e60ce-139">合作伙伴的此租户的状态。</span><span class="sxs-lookup"><span data-stu-id="e60ce-139">Partner state of this tenant.</span></span> <span data-ttu-id="e60ce-140">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="e60ce-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="e60ce-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="e60ce-141">partnerAppType</span></span>|[<span data-ttu-id="e60ce-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="e60ce-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="e60ce-143">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="e60ce-143">Partner App type.</span></span> <span data-ttu-id="e60ce-144">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="e60ce-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="e60ce-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="e60ce-145">singleTenantAppId</span></span>|<span data-ttu-id="e60ce-146">String</span><span class="sxs-lookup"><span data-stu-id="e60ce-146">String</span></span>|<span data-ttu-id="e60ce-147">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="e60ce-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="e60ce-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e60ce-148">displayName</span></span>|<span data-ttu-id="e60ce-149">String</span><span class="sxs-lookup"><span data-stu-id="e60ce-149">String</span></span>|<span data-ttu-id="e60ce-150">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="e60ce-150">Partner display name</span></span>|
|<span data-ttu-id="e60ce-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="e60ce-151">isConfigured</span></span>|<span data-ttu-id="e60ce-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60ce-152">Boolean</span></span>|<span data-ttu-id="e60ce-153">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="e60ce-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="e60ce-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="e60ce-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="e60ce-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e60ce-155">DateTimeOffset</span></span>|<span data-ttu-id="e60ce-156">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="e60ce-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="e60ce-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="e60ce-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="e60ce-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e60ce-158">DateTimeOffset</span></span>|<span data-ttu-id="e60ce-159">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="e60ce-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="e60ce-160">响应</span><span class="sxs-lookup"><span data-stu-id="e60ce-160">Response</span></span>
<span data-ttu-id="e60ce-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e60ce-161">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e60ce-162">示例</span><span class="sxs-lookup"><span data-stu-id="e60ce-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="e60ce-163">请求</span><span class="sxs-lookup"><span data-stu-id="e60ce-163">Request</span></span>
<span data-ttu-id="e60ce-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e60ce-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e60ce-165">响应</span><span class="sxs-lookup"><span data-stu-id="e60ce-165">Response</span></span>
<span data-ttu-id="e60ce-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e60ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



