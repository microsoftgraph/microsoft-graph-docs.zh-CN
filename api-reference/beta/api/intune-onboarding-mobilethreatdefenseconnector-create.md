---
title: 创建 mobileThreatDefenseConnector
description: 创建新的 mobileThreatDefenseConnector 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68da053288b635454c3343bc2fd4795c51456095
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418608"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="b2454-103">创建 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="b2454-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="b2454-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b2454-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b2454-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b2454-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2454-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2454-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2454-107">创建新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2454-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2454-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2454-108">Prerequisites</span></span>
<span data-ttu-id="b2454-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b2454-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2454-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2454-111">Permission type</span></span>|<span data-ttu-id="b2454-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2454-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2454-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2454-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2454-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2454-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b2454-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2454-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2454-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2454-116">Not supported.</span></span>|
|<span data-ttu-id="b2454-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2454-117">Application</span></span>|<span data-ttu-id="b2454-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2454-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2454-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2454-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="b2454-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2454-120">Request headers</span></span>
|<span data-ttu-id="b2454-121">标头</span><span class="sxs-lookup"><span data-stu-id="b2454-121">Header</span></span>|<span data-ttu-id="b2454-122">值</span><span class="sxs-lookup"><span data-stu-id="b2454-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2454-123">授权</span><span class="sxs-lookup"><span data-stu-id="b2454-123">Authorization</span></span>|<span data-ttu-id="b2454-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2454-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2454-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2454-125">Accept</span></span>|<span data-ttu-id="b2454-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2454-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2454-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2454-127">Request body</span></span>
<span data-ttu-id="b2454-128">在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2454-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="b2454-129">下表显示创建 mobileThreatDefenseConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2454-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="b2454-130">属性</span><span class="sxs-lookup"><span data-stu-id="b2454-130">Property</span></span>|<span data-ttu-id="b2454-131">类型</span><span class="sxs-lookup"><span data-stu-id="b2454-131">Type</span></span>|<span data-ttu-id="b2454-132">说明</span><span class="sxs-lookup"><span data-stu-id="b2454-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2454-133">id</span><span class="sxs-lookup"><span data-stu-id="b2454-133">id</span></span>|<span data-ttu-id="b2454-134">String</span><span class="sxs-lookup"><span data-stu-id="b2454-134">String</span></span>|<span data-ttu-id="b2454-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b2454-135">Not yet documented</span></span>|
|<span data-ttu-id="b2454-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b2454-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b2454-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2454-137">DateTimeOffset</span></span>|<span data-ttu-id="b2454-138">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="b2454-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="b2454-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="b2454-139">partnerState</span></span>|[<span data-ttu-id="b2454-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="b2454-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="b2454-141">数据同步合作伙伴为此帐户的的状态。</span><span class="sxs-lookup"><span data-stu-id="b2454-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="b2454-142">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="b2454-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="b2454-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="b2454-143">androidEnabled</span></span>|<span data-ttu-id="b2454-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-144">Boolean</span></span>|<span data-ttu-id="b2454-145">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2454-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="b2454-146">iosEnabled</span></span>|<span data-ttu-id="b2454-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-147">Boolean</span></span>|<span data-ttu-id="b2454-148">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2454-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="b2454-149">windowsEnabled</span></span>|<span data-ttu-id="b2454-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-150">Boolean</span></span>|<span data-ttu-id="b2454-151">用于 Windows，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2454-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="b2454-152">macEnabled</span></span>|<span data-ttu-id="b2454-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-153">Boolean</span></span>|<span data-ttu-id="b2454-154">用于 Mac，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2454-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2454-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2454-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-156">Boolean</span></span>|<span data-ttu-id="b2454-157">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2454-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2454-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2454-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-159">Boolean</span></span>|<span data-ttu-id="b2454-160">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2454-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2454-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2454-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-162">Boolean</span></span>|<span data-ttu-id="b2454-163">对于 Windows，设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2454-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2454-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2454-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-165">Boolean</span></span>|<span data-ttu-id="b2454-166">用于 Mac，获取或设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="b2454-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2454-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="b2454-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="b2454-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-168">Boolean</span></span>|<span data-ttu-id="b2454-169">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="b2454-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="b2454-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="b2454-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="b2454-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b2454-171">Int32</span></span>|<span data-ttu-id="b2454-172">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="b2454-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="b2454-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="b2454-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="b2454-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2454-174">Boolean</span></span>|<span data-ttu-id="b2454-175">对于 IOS 设备，允许管理员配置是否从 Intune 数据同步合作伙伴中可能还收集有关已安装应用程序的元数据</span><span class="sxs-lookup"><span data-stu-id="b2454-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="b2454-176">响应</span><span class="sxs-lookup"><span data-stu-id="b2454-176">Response</span></span>
<span data-ttu-id="b2454-177">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2454-177">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2454-178">示例</span><span class="sxs-lookup"><span data-stu-id="b2454-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2454-179">请求</span><span class="sxs-lookup"><span data-stu-id="b2454-179">Request</span></span>
<span data-ttu-id="b2454-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2454-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2454-181">响应</span><span class="sxs-lookup"><span data-stu-id="b2454-181">Response</span></span>
<span data-ttu-id="b2454-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2454-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




