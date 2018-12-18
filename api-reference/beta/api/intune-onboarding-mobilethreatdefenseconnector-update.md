---
title: 更新 mobileThreatDefenseConnector
description: 更新 mobileThreatDefenseConnector 对象的属性。
author: tfitzmac
ms.openlocfilehash: 53e6cb6a4d3fc794bb86f031e2d405532e529ad1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336279"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="53a21-103">更新 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="53a21-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="53a21-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="53a21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53a21-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53a21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53a21-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="53a21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53a21-107">更新 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53a21-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53a21-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="53a21-108">Prerequisites</span></span>
<span data-ttu-id="53a21-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="53a21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53a21-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53a21-111">Permission type</span></span>|<span data-ttu-id="53a21-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53a21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53a21-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53a21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53a21-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53a21-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53a21-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53a21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53a21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53a21-116">Not supported.</span></span>|
|<span data-ttu-id="53a21-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53a21-117">Application</span></span>|<span data-ttu-id="53a21-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="53a21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53a21-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53a21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="53a21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53a21-120">Request headers</span></span>
|<span data-ttu-id="53a21-121">标头</span><span class="sxs-lookup"><span data-stu-id="53a21-121">Header</span></span>|<span data-ttu-id="53a21-122">值</span><span class="sxs-lookup"><span data-stu-id="53a21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53a21-123">授权</span><span class="sxs-lookup"><span data-stu-id="53a21-123">Authorization</span></span>|<span data-ttu-id="53a21-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53a21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53a21-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53a21-125">Accept</span></span>|<span data-ttu-id="53a21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53a21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53a21-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53a21-127">Request body</span></span>
<span data-ttu-id="53a21-128">在请求正文中，提供 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53a21-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="53a21-129">下表显示了创建 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53a21-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="53a21-130">属性</span><span class="sxs-lookup"><span data-stu-id="53a21-130">Property</span></span>|<span data-ttu-id="53a21-131">类型</span><span class="sxs-lookup"><span data-stu-id="53a21-131">Type</span></span>|<span data-ttu-id="53a21-132">说明</span><span class="sxs-lookup"><span data-stu-id="53a21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53a21-133">id</span><span class="sxs-lookup"><span data-stu-id="53a21-133">id</span></span>|<span data-ttu-id="53a21-134">字符串</span><span class="sxs-lookup"><span data-stu-id="53a21-134">String</span></span>|<span data-ttu-id="53a21-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="53a21-135">Not yet documented</span></span>|
|<span data-ttu-id="53a21-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="53a21-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="53a21-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a21-137">DateTimeOffset</span></span>|<span data-ttu-id="53a21-138">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="53a21-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="53a21-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="53a21-139">partnerState</span></span>|[<span data-ttu-id="53a21-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="53a21-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="53a21-141">数据同步合作伙伴为此帐户的的状态。</span><span class="sxs-lookup"><span data-stu-id="53a21-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="53a21-142">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="53a21-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="53a21-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="53a21-143">androidEnabled</span></span>|<span data-ttu-id="53a21-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-144">Boolean</span></span>|<span data-ttu-id="53a21-145">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="53a21-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="53a21-146">iosEnabled</span></span>|<span data-ttu-id="53a21-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-147">Boolean</span></span>|<span data-ttu-id="53a21-148">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="53a21-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="53a21-149">windowsEnabled</span></span>|<span data-ttu-id="53a21-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-150">Boolean</span></span>|<span data-ttu-id="53a21-151">用于 Windows，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="53a21-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="53a21-152">macEnabled</span></span>|<span data-ttu-id="53a21-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-153">Boolean</span></span>|<span data-ttu-id="53a21-154">用于 Mac，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="53a21-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="53a21-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="53a21-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-156">Boolean</span></span>|<span data-ttu-id="53a21-157">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="53a21-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="53a21-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="53a21-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-159">Boolean</span></span>|<span data-ttu-id="53a21-160">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="53a21-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="53a21-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="53a21-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-162">Boolean</span></span>|<span data-ttu-id="53a21-163">对于 Windows，设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="53a21-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="53a21-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="53a21-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-165">Boolean</span></span>|<span data-ttu-id="53a21-166">用于 Mac，获取或设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="53a21-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="53a21-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="53a21-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="53a21-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-168">Boolean</span></span>|<span data-ttu-id="53a21-169">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="53a21-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="53a21-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="53a21-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="53a21-171">Int32</span><span class="sxs-lookup"><span data-stu-id="53a21-171">Int32</span></span>|<span data-ttu-id="53a21-172">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="53a21-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="53a21-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="53a21-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="53a21-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a21-174">Boolean</span></span>|<span data-ttu-id="53a21-175">对于 IOS 设备，允许管理员配置是否从 Intune 数据同步合作伙伴中可能还收集有关已安装应用程序的元数据</span><span class="sxs-lookup"><span data-stu-id="53a21-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="53a21-176">响应</span><span class="sxs-lookup"><span data-stu-id="53a21-176">Response</span></span>
<span data-ttu-id="53a21-177">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53a21-177">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53a21-178">示例</span><span class="sxs-lookup"><span data-stu-id="53a21-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="53a21-179">请求</span><span class="sxs-lookup"><span data-stu-id="53a21-179">Request</span></span>
<span data-ttu-id="53a21-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53a21-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 555

{
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

### <a name="response"></a><span data-ttu-id="53a21-181">响应</span><span class="sxs-lookup"><span data-stu-id="53a21-181">Response</span></span>
<span data-ttu-id="53a21-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53a21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





