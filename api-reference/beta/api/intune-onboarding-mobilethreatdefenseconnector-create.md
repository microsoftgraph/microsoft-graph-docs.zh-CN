---
title: 创建 mobileThreatDefenseConnector
description: 创建新的 mobileThreatDefenseConnector 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6653d9eb4abc5705eaa8a2dff61c0a758e9a05cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352579"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="4dc6b-103">创建 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="4dc6b-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="4dc6b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dc6b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc6b-106">创建新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dc6b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4dc6b-107">Prerequisites</span></span>
<span data-ttu-id="4dc6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc6b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dc6b-110">Permission type</span></span>|<span data-ttu-id="4dc6b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4dc6b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dc6b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dc6b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc6b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dc6b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dc6b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-115">Not supported.</span></span>|
|<span data-ttu-id="4dc6b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dc6b-116">Application</span></span>|<span data-ttu-id="4dc6b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc6b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dc6b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dc6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4dc6b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dc6b-119">Request headers</span></span>
|<span data-ttu-id="4dc6b-120">标头</span><span class="sxs-lookup"><span data-stu-id="4dc6b-120">Header</span></span>|<span data-ttu-id="4dc6b-121">值</span><span class="sxs-lookup"><span data-stu-id="4dc6b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dc6b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dc6b-122">Authorization</span></span>|<span data-ttu-id="4dc6b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dc6b-124">接受</span><span class="sxs-lookup"><span data-stu-id="4dc6b-124">Accept</span></span>|<span data-ttu-id="4dc6b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dc6b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc6b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dc6b-126">Request body</span></span>
<span data-ttu-id="4dc6b-127">在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="4dc6b-128">下表显示创建 mobileThreatDefenseConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="4dc6b-129">属性</span><span class="sxs-lookup"><span data-stu-id="4dc6b-129">Property</span></span>|<span data-ttu-id="4dc6b-130">类型</span><span class="sxs-lookup"><span data-stu-id="4dc6b-130">Type</span></span>|<span data-ttu-id="4dc6b-131">说明</span><span class="sxs-lookup"><span data-stu-id="4dc6b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc6b-132">id</span><span class="sxs-lookup"><span data-stu-id="4dc6b-132">id</span></span>|<span data-ttu-id="4dc6b-133">String</span><span class="sxs-lookup"><span data-stu-id="4dc6b-133">String</span></span>|<span data-ttu-id="4dc6b-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4dc6b-134">Not yet documented</span></span>|
|<span data-ttu-id="4dc6b-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4dc6b-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4dc6b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dc6b-136">DateTimeOffset</span></span>|<span data-ttu-id="4dc6b-137">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="4dc6b-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="4dc6b-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="4dc6b-138">partnerState</span></span>|[<span data-ttu-id="4dc6b-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4dc6b-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="4dc6b-140">此帐户的数据同步合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="4dc6b-141">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="4dc6b-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="4dc6b-142">androidEnabled</span></span>|<span data-ttu-id="4dc6b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-143">Boolean</span></span>|<span data-ttu-id="4dc6b-144">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4dc6b-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="4dc6b-145">iosEnabled</span></span>|<span data-ttu-id="4dc6b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-146">Boolean</span></span>|<span data-ttu-id="4dc6b-147">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4dc6b-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="4dc6b-148">windowsEnabled</span></span>|<span data-ttu-id="4dc6b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-149">Boolean</span></span>|<span data-ttu-id="4dc6b-150">对于 Windows, 获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4dc6b-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="4dc6b-151">macEnabled</span></span>|<span data-ttu-id="4dc6b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-152">Boolean</span></span>|<span data-ttu-id="4dc6b-153">对于 Mac, 获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4dc6b-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4dc6b-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4dc6b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-155">Boolean</span></span>|<span data-ttu-id="4dc6b-156">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4dc6b-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4dc6b-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4dc6b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-158">Boolean</span></span>|<span data-ttu-id="4dc6b-159">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4dc6b-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4dc6b-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4dc6b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-161">Boolean</span></span>|<span data-ttu-id="4dc6b-162">对于 Windows, 在将设备标记为合规之前, 设置 Intune 是否必须接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4dc6b-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4dc6b-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4dc6b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-164">Boolean</span></span>|<span data-ttu-id="4dc6b-165">对于 Mac, 获取或设置 Intune 是否必须在标记符合设备的之前从数据同步合作伙伴接收数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4dc6b-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="4dc6b-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="4dc6b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-167">Boolean</span></span>|<span data-ttu-id="4dc6b-168">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="4dc6b-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="4dc6b-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="4dc6b-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="4dc6b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc6b-170">Int32</span></span>|<span data-ttu-id="4dc6b-171">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="4dc6b-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="4dc6b-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="4dc6b-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="4dc6b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc6b-173">Boolean</span></span>|<span data-ttu-id="4dc6b-174">对于 IOS 设备, 管理员可以配置数据同步合作伙伴是否可以从 Intune 收集有关已安装应用程序的元数据</span><span class="sxs-lookup"><span data-stu-id="4dc6b-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="4dc6b-175">响应</span><span class="sxs-lookup"><span data-stu-id="4dc6b-175">Response</span></span>
<span data-ttu-id="4dc6b-176">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-176">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc6b-177">示例</span><span class="sxs-lookup"><span data-stu-id="4dc6b-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dc6b-178">请求</span><span class="sxs-lookup"><span data-stu-id="4dc6b-178">Request</span></span>
<span data-ttu-id="4dc6b-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a><span data-ttu-id="4dc6b-180">响应</span><span class="sxs-lookup"><span data-stu-id="4dc6b-180">Response</span></span>
<span data-ttu-id="4dc6b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dc6b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```






