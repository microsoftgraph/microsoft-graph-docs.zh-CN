---
title: 创建 mobileThreatDefenseConnector
description: 创建新的 mobileThreatDefenseConnector 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c20146a7c6a84526382aa610d7cb632ba9eb5aef
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731188"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="22d5e-103">创建 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="22d5e-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="22d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22d5e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22d5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22d5e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22d5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d5e-107">创建新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22d5e-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22d5e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="22d5e-108">Prerequisites</span></span>
<span data-ttu-id="22d5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d5e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="22d5e-111">Permission type</span></span>|<span data-ttu-id="22d5e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="22d5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d5e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22d5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22d5e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d5e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22d5e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22d5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22d5e-116">Not supported.</span></span>|
|<span data-ttu-id="22d5e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="22d5e-117">Application</span></span>|<span data-ttu-id="22d5e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d5e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d5e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22d5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="22d5e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22d5e-120">Request headers</span></span>
|<span data-ttu-id="22d5e-121">标头</span><span class="sxs-lookup"><span data-stu-id="22d5e-121">Header</span></span>|<span data-ttu-id="22d5e-122">值</span><span class="sxs-lookup"><span data-stu-id="22d5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22d5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d5e-123">Authorization</span></span>|<span data-ttu-id="22d5e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22d5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22d5e-125">接受</span><span class="sxs-lookup"><span data-stu-id="22d5e-125">Accept</span></span>|<span data-ttu-id="22d5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22d5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22d5e-127">Request body</span></span>
<span data-ttu-id="22d5e-128">在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22d5e-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="22d5e-129">下表显示创建 mobileThreatDefenseConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="22d5e-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="22d5e-130">属性</span><span class="sxs-lookup"><span data-stu-id="22d5e-130">Property</span></span>|<span data-ttu-id="22d5e-131">类型</span><span class="sxs-lookup"><span data-stu-id="22d5e-131">Type</span></span>|<span data-ttu-id="22d5e-132">说明</span><span class="sxs-lookup"><span data-stu-id="22d5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d5e-133">id</span><span class="sxs-lookup"><span data-stu-id="22d5e-133">id</span></span>|<span data-ttu-id="22d5e-134">String</span><span class="sxs-lookup"><span data-stu-id="22d5e-134">String</span></span>|<span data-ttu-id="22d5e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="22d5e-135">Not yet documented</span></span>|
|<span data-ttu-id="22d5e-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="22d5e-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="22d5e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d5e-137">DateTimeOffset</span></span>|<span data-ttu-id="22d5e-138">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="22d5e-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="22d5e-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="22d5e-139">partnerState</span></span>|[<span data-ttu-id="22d5e-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="22d5e-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="22d5e-141">此帐户的数据同步合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="22d5e-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="22d5e-142">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="22d5e-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="22d5e-143">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="22d5e-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="22d5e-144">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-144">Boolean</span></span>|<span data-ttu-id="22d5e-145">对于 Android，请设置是否应在移动应用程序管理 (MAM) 评估期间使用来自数据同步合作伙伴的数据。</span><span class="sxs-lookup"><span data-stu-id="22d5e-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="22d5e-146">对于移动应用程序管理 (MAM) 评估，仅可为每个平台启用一个合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="22d5e-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="22d5e-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="22d5e-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="22d5e-148">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-148">Boolean</span></span>|<span data-ttu-id="22d5e-149">对于 IOS，获取或设置是否应在移动应用程序管理 (MAM) 评估期间使用来自数据同步合作伙伴的数据。</span><span class="sxs-lookup"><span data-stu-id="22d5e-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="22d5e-150">对于移动应用程序管理 (MAM) 评估，仅可为每个平台启用一个合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="22d5e-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="22d5e-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="22d5e-151">androidEnabled</span></span>|<span data-ttu-id="22d5e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="22d5e-152">Boolean</span></span>|<span data-ttu-id="22d5e-153">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="22d5e-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="22d5e-154">iosEnabled</span></span>|<span data-ttu-id="22d5e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="22d5e-155">Boolean</span></span>|<span data-ttu-id="22d5e-156">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="22d5e-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="22d5e-157">windowsEnabled</span></span>|<span data-ttu-id="22d5e-158">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-158">Boolean</span></span>|<span data-ttu-id="22d5e-159">对于 Windows，获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="22d5e-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="22d5e-160">macEnabled</span></span>|<span data-ttu-id="22d5e-161">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-161">Boolean</span></span>|<span data-ttu-id="22d5e-162">对于 Mac，获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="22d5e-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="22d5e-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="22d5e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="22d5e-164">Boolean</span></span>|<span data-ttu-id="22d5e-165">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="22d5e-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="22d5e-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="22d5e-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="22d5e-167">Boolean</span></span>|<span data-ttu-id="22d5e-168">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="22d5e-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="22d5e-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="22d5e-170">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-170">Boolean</span></span>|<span data-ttu-id="22d5e-171">对于 Windows，在将设备标记为合规之前，设置 Intune 是否必须接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="22d5e-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="22d5e-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="22d5e-173">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-173">Boolean</span></span>|<span data-ttu-id="22d5e-174">对于 Mac，获取或设置 Intune 是否必须在标记符合设备的之前从数据同步合作伙伴接收数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="22d5e-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="22d5e-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="22d5e-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="22d5e-176">Boolean</span></span>|<span data-ttu-id="22d5e-177">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="22d5e-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="22d5e-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="22d5e-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="22d5e-179">Int32</span><span class="sxs-lookup"><span data-stu-id="22d5e-179">Int32</span></span>|<span data-ttu-id="22d5e-180">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="22d5e-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="22d5e-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="22d5e-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="22d5e-182">布尔</span><span class="sxs-lookup"><span data-stu-id="22d5e-182">Boolean</span></span>|<span data-ttu-id="22d5e-183">对于 IOS 设备，管理员可以配置数据同步合作伙伴是否可以从 Intune 收集有关已安装应用程序的元数据</span><span class="sxs-lookup"><span data-stu-id="22d5e-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="22d5e-184">响应</span><span class="sxs-lookup"><span data-stu-id="22d5e-184">Response</span></span>
<span data-ttu-id="22d5e-185">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22d5e-185">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d5e-186">示例</span><span class="sxs-lookup"><span data-stu-id="22d5e-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="22d5e-187">请求</span><span class="sxs-lookup"><span data-stu-id="22d5e-187">Request</span></span>
<span data-ttu-id="22d5e-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22d5e-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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

### <a name="response"></a><span data-ttu-id="22d5e-189">响应</span><span class="sxs-lookup"><span data-stu-id="22d5e-189">Response</span></span>
<span data-ttu-id="22d5e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22d5e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 775

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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





