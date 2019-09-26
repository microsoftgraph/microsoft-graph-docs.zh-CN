---
title: 更新 mobileThreatDefenseConnector
description: 更新 mobileThreatDefenseConnector 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df2546c8c011ac68043f969cfd7ddd78323ca2db
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190430"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="35f9d-103">更新 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="35f9d-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="35f9d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35f9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35f9d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35f9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f9d-106">更新 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35f9d-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f9d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="35f9d-107">Prerequisites</span></span>
<span data-ttu-id="35f9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f9d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35f9d-110">Permission type</span></span>|<span data-ttu-id="35f9d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35f9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f9d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35f9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35f9d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f9d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="35f9d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35f9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f9d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35f9d-115">Not supported.</span></span>|
|<span data-ttu-id="35f9d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="35f9d-116">Application</span></span>|<span data-ttu-id="35f9d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f9d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f9d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35f9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="35f9d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="35f9d-119">Request headers</span></span>
|<span data-ttu-id="35f9d-120">标头</span><span class="sxs-lookup"><span data-stu-id="35f9d-120">Header</span></span>|<span data-ttu-id="35f9d-121">值</span><span class="sxs-lookup"><span data-stu-id="35f9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f9d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35f9d-122">Authorization</span></span>|<span data-ttu-id="35f9d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35f9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f9d-124">接受</span><span class="sxs-lookup"><span data-stu-id="35f9d-124">Accept</span></span>|<span data-ttu-id="35f9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35f9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f9d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="35f9d-126">Request body</span></span>
<span data-ttu-id="35f9d-127">在请求正文中，提供 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35f9d-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="35f9d-128">下表显示了创建 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35f9d-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="35f9d-129">属性</span><span class="sxs-lookup"><span data-stu-id="35f9d-129">Property</span></span>|<span data-ttu-id="35f9d-130">类型</span><span class="sxs-lookup"><span data-stu-id="35f9d-130">Type</span></span>|<span data-ttu-id="35f9d-131">说明</span><span class="sxs-lookup"><span data-stu-id="35f9d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f9d-132">id</span><span class="sxs-lookup"><span data-stu-id="35f9d-132">id</span></span>|<span data-ttu-id="35f9d-133">String</span><span class="sxs-lookup"><span data-stu-id="35f9d-133">String</span></span>|<span data-ttu-id="35f9d-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="35f9d-134">Not yet documented</span></span>|
|<span data-ttu-id="35f9d-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="35f9d-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="35f9d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f9d-136">DateTimeOffset</span></span>|<span data-ttu-id="35f9d-137">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="35f9d-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="35f9d-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="35f9d-138">partnerState</span></span>|[<span data-ttu-id="35f9d-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="35f9d-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="35f9d-140">此帐户的数据同步合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="35f9d-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="35f9d-141">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="35f9d-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="35f9d-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="35f9d-142">androidEnabled</span></span>|<span data-ttu-id="35f9d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-143">Boolean</span></span>|<span data-ttu-id="35f9d-144">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="35f9d-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="35f9d-145">iosEnabled</span></span>|<span data-ttu-id="35f9d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-146">Boolean</span></span>|<span data-ttu-id="35f9d-147">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="35f9d-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="35f9d-148">windowsEnabled</span></span>|<span data-ttu-id="35f9d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-149">Boolean</span></span>|<span data-ttu-id="35f9d-150">对于 Windows，获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="35f9d-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="35f9d-151">macEnabled</span></span>|<span data-ttu-id="35f9d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-152">Boolean</span></span>|<span data-ttu-id="35f9d-153">对于 Mac，获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="35f9d-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="35f9d-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="35f9d-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-155">Boolean</span></span>|<span data-ttu-id="35f9d-156">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="35f9d-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="35f9d-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="35f9d-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-158">Boolean</span></span>|<span data-ttu-id="35f9d-159">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="35f9d-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="35f9d-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="35f9d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-161">Boolean</span></span>|<span data-ttu-id="35f9d-162">对于 Windows，在将设备标记为合规之前，设置 Intune 是否必须接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="35f9d-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="35f9d-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="35f9d-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-164">Boolean</span></span>|<span data-ttu-id="35f9d-165">对于 Mac，获取或设置 Intune 是否必须在标记符合设备的之前从数据同步合作伙伴接收数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="35f9d-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="35f9d-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="35f9d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-167">Boolean</span></span>|<span data-ttu-id="35f9d-168">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="35f9d-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="35f9d-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="35f9d-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="35f9d-170">Int32</span><span class="sxs-lookup"><span data-stu-id="35f9d-170">Int32</span></span>|<span data-ttu-id="35f9d-171">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="35f9d-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="35f9d-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="35f9d-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="35f9d-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f9d-173">Boolean</span></span>|<span data-ttu-id="35f9d-174">对于 IOS 设备，管理员可以配置数据同步合作伙伴是否可以从 Intune 收集有关已安装应用程序的元数据</span><span class="sxs-lookup"><span data-stu-id="35f9d-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="35f9d-175">响应</span><span class="sxs-lookup"><span data-stu-id="35f9d-175">Response</span></span>
<span data-ttu-id="35f9d-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35f9d-176">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f9d-177">示例</span><span class="sxs-lookup"><span data-stu-id="35f9d-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f9d-178">请求</span><span class="sxs-lookup"><span data-stu-id="35f9d-178">Request</span></span>
<span data-ttu-id="35f9d-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35f9d-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
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

### <a name="response"></a><span data-ttu-id="35f9d-180">响应</span><span class="sxs-lookup"><span data-stu-id="35f9d-180">Response</span></span>
<span data-ttu-id="35f9d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35f9d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




