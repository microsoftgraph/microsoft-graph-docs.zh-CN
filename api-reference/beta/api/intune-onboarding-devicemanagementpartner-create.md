---
title: 创建 deviceManagementPartner
description: 创建新的 deviceManagementPartner 对象。
author: tfitzmac
ms.openlocfilehash: f8778ff23ed5990e1749bc36122587ef20488417
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333549"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="b84e3-103">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b84e3-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="b84e3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b84e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b84e3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b84e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b84e3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b84e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b84e3-107">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b84e3-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b84e3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b84e3-108">Prerequisites</span></span>
<span data-ttu-id="b84e3-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b84e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b84e3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b84e3-111">Permission type</span></span>|<span data-ttu-id="b84e3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b84e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b84e3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b84e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b84e3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b84e3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b84e3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b84e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b84e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b84e3-116">Not supported.</span></span>|
|<span data-ttu-id="b84e3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b84e3-117">Application</span></span>|<span data-ttu-id="b84e3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b84e3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b84e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b84e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="b84e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b84e3-120">Request headers</span></span>
|<span data-ttu-id="b84e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="b84e3-121">Header</span></span>|<span data-ttu-id="b84e3-122">值</span><span class="sxs-lookup"><span data-stu-id="b84e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b84e3-123">授权</span><span class="sxs-lookup"><span data-stu-id="b84e3-123">Authorization</span></span>|<span data-ttu-id="b84e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b84e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b84e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b84e3-125">Accept</span></span>|<span data-ttu-id="b84e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b84e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b84e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b84e3-127">Request body</span></span>
<span data-ttu-id="b84e3-128">在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b84e3-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="b84e3-129">下表显示创建 deviceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b84e3-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="b84e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="b84e3-130">Property</span></span>|<span data-ttu-id="b84e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="b84e3-131">Type</span></span>|<span data-ttu-id="b84e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="b84e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b84e3-133">id</span><span class="sxs-lookup"><span data-stu-id="b84e3-133">id</span></span>|<span data-ttu-id="b84e3-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b84e3-134">String</span></span>|<span data-ttu-id="b84e3-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b84e3-135">Not yet documented</span></span>|
|<span data-ttu-id="b84e3-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b84e3-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b84e3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84e3-137">DateTimeOffset</span></span>|<span data-ttu-id="b84e3-138">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="b84e3-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="b84e3-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="b84e3-139">partnerState</span></span>|[<span data-ttu-id="b84e3-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="b84e3-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="b84e3-141">合作伙伴的此租户的状态。</span><span class="sxs-lookup"><span data-stu-id="b84e3-141">Partner state of this tenant.</span></span> <span data-ttu-id="b84e3-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="b84e3-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="b84e3-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="b84e3-143">partnerAppType</span></span>|[<span data-ttu-id="b84e3-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="b84e3-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="b84e3-145">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="b84e3-145">Partner App type.</span></span> <span data-ttu-id="b84e3-146">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="b84e3-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="b84e3-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="b84e3-147">singleTenantAppId</span></span>|<span data-ttu-id="b84e3-148">String</span><span class="sxs-lookup"><span data-stu-id="b84e3-148">String</span></span>|<span data-ttu-id="b84e3-149">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="b84e3-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="b84e3-150">displayName</span><span class="sxs-lookup"><span data-stu-id="b84e3-150">displayName</span></span>|<span data-ttu-id="b84e3-151">String</span><span class="sxs-lookup"><span data-stu-id="b84e3-151">String</span></span>|<span data-ttu-id="b84e3-152">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="b84e3-152">Partner display name</span></span>|
|<span data-ttu-id="b84e3-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="b84e3-153">isConfigured</span></span>|<span data-ttu-id="b84e3-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b84e3-154">Boolean</span></span>|<span data-ttu-id="b84e3-155">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b84e3-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="b84e3-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="b84e3-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="b84e3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84e3-157">DateTimeOffset</span></span>|<span data-ttu-id="b84e3-158">采用 UTC 时将删除 PartnerDevices 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b84e3-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="b84e3-159">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="b84e3-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="b84e3-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="b84e3-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="b84e3-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84e3-161">DateTimeOffset</span></span>|<span data-ttu-id="b84e3-162">采用 UTC PartnerDevices 将标记为不符合时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b84e3-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="b84e3-163">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="b84e3-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="b84e3-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="b84e3-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="b84e3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84e3-165">DateTimeOffset</span></span>|<span data-ttu-id="b84e3-166">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="b84e3-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="b84e3-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="b84e3-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="b84e3-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84e3-168">DateTimeOffset</span></span>|<span data-ttu-id="b84e3-169">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="b84e3-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="b84e3-170">响应</span><span class="sxs-lookup"><span data-stu-id="b84e3-170">Response</span></span>
<span data-ttu-id="b84e3-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b84e3-171">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b84e3-172">示例</span><span class="sxs-lookup"><span data-stu-id="b84e3-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="b84e3-173">请求</span><span class="sxs-lookup"><span data-stu-id="b84e3-173">Request</span></span>
<span data-ttu-id="b84e3-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b84e3-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="b84e3-175">响应</span><span class="sxs-lookup"><span data-stu-id="b84e3-175">Response</span></span>
<span data-ttu-id="b84e3-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b84e3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





