---
title: 更新 deviceManagementPartner
description: 更新 deviceManagementPartner 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 26646fc7afb04fb577f8cbf7d160869de8889e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956442"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="77587-103">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="77587-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="77587-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="77587-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77587-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="77587-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77587-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="77587-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77587-107">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77587-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77587-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77587-108">Prerequisites</span></span>
<span data-ttu-id="77587-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="77587-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77587-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77587-111">Permission type</span></span>|<span data-ttu-id="77587-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77587-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77587-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77587-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77587-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77587-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77587-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77587-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77587-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77587-116">Not supported.</span></span>|
|<span data-ttu-id="77587-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77587-117">Application</span></span>|<span data-ttu-id="77587-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="77587-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77587-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77587-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="77587-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="77587-120">Request headers</span></span>
|<span data-ttu-id="77587-121">标头</span><span class="sxs-lookup"><span data-stu-id="77587-121">Header</span></span>|<span data-ttu-id="77587-122">值</span><span class="sxs-lookup"><span data-stu-id="77587-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77587-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77587-123">Authorization</span></span>|<span data-ttu-id="77587-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77587-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77587-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77587-125">Accept</span></span>|<span data-ttu-id="77587-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77587-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77587-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77587-127">Request body</span></span>
<span data-ttu-id="77587-128">在请求正文中，提供 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77587-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="77587-129">下表显示创建 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="77587-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="77587-130">属性</span><span class="sxs-lookup"><span data-stu-id="77587-130">Property</span></span>|<span data-ttu-id="77587-131">类型</span><span class="sxs-lookup"><span data-stu-id="77587-131">Type</span></span>|<span data-ttu-id="77587-132">说明</span><span class="sxs-lookup"><span data-stu-id="77587-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77587-133">id</span><span class="sxs-lookup"><span data-stu-id="77587-133">id</span></span>|<span data-ttu-id="77587-134">字符串</span><span class="sxs-lookup"><span data-stu-id="77587-134">String</span></span>|<span data-ttu-id="77587-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="77587-135">Not yet documented</span></span>|
|<span data-ttu-id="77587-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="77587-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="77587-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77587-137">DateTimeOffset</span></span>|<span data-ttu-id="77587-138">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="77587-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="77587-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="77587-139">partnerState</span></span>|[<span data-ttu-id="77587-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="77587-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="77587-141">合作伙伴的此租户的状态。</span><span class="sxs-lookup"><span data-stu-id="77587-141">Partner state of this tenant.</span></span> <span data-ttu-id="77587-142">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="77587-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="77587-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="77587-143">partnerAppType</span></span>|[<span data-ttu-id="77587-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="77587-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="77587-145">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="77587-145">Partner App type.</span></span> <span data-ttu-id="77587-146">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="77587-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="77587-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="77587-147">singleTenantAppId</span></span>|<span data-ttu-id="77587-148">String</span><span class="sxs-lookup"><span data-stu-id="77587-148">String</span></span>|<span data-ttu-id="77587-149">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="77587-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="77587-150">displayName</span><span class="sxs-lookup"><span data-stu-id="77587-150">displayName</span></span>|<span data-ttu-id="77587-151">String</span><span class="sxs-lookup"><span data-stu-id="77587-151">String</span></span>|<span data-ttu-id="77587-152">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="77587-152">Partner display name</span></span>|
|<span data-ttu-id="77587-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="77587-153">isConfigured</span></span>|<span data-ttu-id="77587-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="77587-154">Boolean</span></span>|<span data-ttu-id="77587-155">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="77587-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="77587-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="77587-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="77587-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77587-157">DateTimeOffset</span></span>|<span data-ttu-id="77587-158">采用 UTC 时将删除 PartnerDevices 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="77587-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="77587-159">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="77587-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="77587-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="77587-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="77587-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77587-161">DateTimeOffset</span></span>|<span data-ttu-id="77587-162">采用 UTC PartnerDevices 将标记为不符合时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="77587-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="77587-163">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="77587-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="77587-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="77587-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="77587-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77587-165">DateTimeOffset</span></span>|<span data-ttu-id="77587-166">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="77587-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="77587-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="77587-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="77587-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77587-168">DateTimeOffset</span></span>|<span data-ttu-id="77587-169">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="77587-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="77587-170">响应</span><span class="sxs-lookup"><span data-stu-id="77587-170">Response</span></span>
<span data-ttu-id="77587-171">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77587-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77587-172">示例</span><span class="sxs-lookup"><span data-stu-id="77587-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="77587-173">请求</span><span class="sxs-lookup"><span data-stu-id="77587-173">Request</span></span>
<span data-ttu-id="77587-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77587-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 602

{
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

### <a name="response"></a><span data-ttu-id="77587-175">响应</span><span class="sxs-lookup"><span data-stu-id="77587-175">Response</span></span>
<span data-ttu-id="77587-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77587-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





