---
title: 创建 mobileThreatDefenseConnector
description: 创建新的 mobileThreatDefenseConnector 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 923505463d3414bcf4650dd3638cf7b37bb33264
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976076"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="d63a7-103">创建 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="d63a7-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="d63a7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d63a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d63a7-105">创建新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d63a7-105">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d63a7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d63a7-106">Prerequisites</span></span>
<span data-ttu-id="d63a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d63a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d63a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d63a7-109">Permission type</span></span>|<span data-ttu-id="d63a7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d63a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d63a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d63a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d63a7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d63a7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d63a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d63a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d63a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d63a7-114">Not supported.</span></span>|
|<span data-ttu-id="d63a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d63a7-115">Application</span></span>|<span data-ttu-id="d63a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d63a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d63a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d63a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="d63a7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d63a7-118">Request headers</span></span>
|<span data-ttu-id="d63a7-119">标头</span><span class="sxs-lookup"><span data-stu-id="d63a7-119">Header</span></span>|<span data-ttu-id="d63a7-120">值</span><span class="sxs-lookup"><span data-stu-id="d63a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d63a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d63a7-121">Authorization</span></span>|<span data-ttu-id="d63a7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d63a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d63a7-123">接受</span><span class="sxs-lookup"><span data-stu-id="d63a7-123">Accept</span></span>|<span data-ttu-id="d63a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d63a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d63a7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d63a7-125">Request body</span></span>
<span data-ttu-id="d63a7-126">在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d63a7-126">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="d63a7-127">下表显示创建 mobileThreatDefenseConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d63a7-127">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="d63a7-128">属性</span><span class="sxs-lookup"><span data-stu-id="d63a7-128">Property</span></span>|<span data-ttu-id="d63a7-129">类型</span><span class="sxs-lookup"><span data-stu-id="d63a7-129">Type</span></span>|<span data-ttu-id="d63a7-130">说明</span><span class="sxs-lookup"><span data-stu-id="d63a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d63a7-131">id</span><span class="sxs-lookup"><span data-stu-id="d63a7-131">id</span></span>|<span data-ttu-id="d63a7-132">String</span><span class="sxs-lookup"><span data-stu-id="d63a7-132">String</span></span>|<span data-ttu-id="d63a7-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d63a7-133">Not yet documented</span></span>|
|<span data-ttu-id="d63a7-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="d63a7-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="d63a7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d63a7-135">DateTimeOffset</span></span>|<span data-ttu-id="d63a7-136">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="d63a7-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="d63a7-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="d63a7-137">partnerState</span></span>|[<span data-ttu-id="d63a7-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="d63a7-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="d63a7-139">此帐户的数据同步合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="d63a7-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="d63a7-140">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="d63a7-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="d63a7-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="d63a7-141">androidEnabled</span></span>|<span data-ttu-id="d63a7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63a7-142">Boolean</span></span>|<span data-ttu-id="d63a7-143">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="d63a7-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="d63a7-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="d63a7-144">iosEnabled</span></span>|<span data-ttu-id="d63a7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63a7-145">Boolean</span></span>|<span data-ttu-id="d63a7-146">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="d63a7-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="d63a7-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="d63a7-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="d63a7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63a7-148">Boolean</span></span>|<span data-ttu-id="d63a7-149">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="d63a7-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="d63a7-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="d63a7-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="d63a7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63a7-151">Boolean</span></span>|<span data-ttu-id="d63a7-152">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="d63a7-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="d63a7-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="d63a7-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="d63a7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63a7-154">Boolean</span></span>|<span data-ttu-id="d63a7-155">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="d63a7-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="d63a7-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="d63a7-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="d63a7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d63a7-157">Int32</span></span>|<span data-ttu-id="d63a7-158">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="d63a7-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="d63a7-159">响应</span><span class="sxs-lookup"><span data-stu-id="d63a7-159">Response</span></span>
<span data-ttu-id="d63a7-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d63a7-160">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d63a7-161">示例</span><span class="sxs-lookup"><span data-stu-id="d63a7-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="d63a7-162">请求</span><span class="sxs-lookup"><span data-stu-id="d63a7-162">Request</span></span>
<span data-ttu-id="d63a7-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d63a7-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="d63a7-164">响应</span><span class="sxs-lookup"><span data-stu-id="d63a7-164">Response</span></span>
<span data-ttu-id="d63a7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d63a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



