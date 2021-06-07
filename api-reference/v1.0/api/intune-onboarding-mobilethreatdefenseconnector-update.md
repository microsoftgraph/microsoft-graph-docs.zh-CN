---
title: 更新 mobileThreatDefenseConnector
description: 更新 mobileThreatDefenseConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c58b8c2838f89360ab19e33c009946b23f3189d5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751466"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="2d039-103">更新 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="2d039-103">Update mobileThreatDefenseConnector</span></span>

<span data-ttu-id="2d039-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d039-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d039-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d039-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d039-106">更新 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2d039-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d039-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d039-107">Prerequisites</span></span>
<span data-ttu-id="2d039-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d039-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d039-110">Permission type</span></span>|<span data-ttu-id="2d039-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d039-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d039-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d039-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d039-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d039-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d039-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d039-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d039-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d039-115">Not supported.</span></span>|
|<span data-ttu-id="2d039-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d039-116">Application</span></span>|<span data-ttu-id="2d039-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d039-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d039-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d039-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="2d039-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d039-119">Request headers</span></span>
|<span data-ttu-id="2d039-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d039-120">Header</span></span>|<span data-ttu-id="2d039-121">值</span><span class="sxs-lookup"><span data-stu-id="2d039-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d039-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d039-122">Authorization</span></span>|<span data-ttu-id="2d039-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d039-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d039-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d039-124">Accept</span></span>|<span data-ttu-id="2d039-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d039-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d039-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d039-126">Request body</span></span>
<span data-ttu-id="2d039-127">在请求正文中，提供 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d039-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="2d039-128">下表显示了创建 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d039-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="2d039-129">属性</span><span class="sxs-lookup"><span data-stu-id="2d039-129">Property</span></span>|<span data-ttu-id="2d039-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d039-130">Type</span></span>|<span data-ttu-id="2d039-131">说明</span><span class="sxs-lookup"><span data-stu-id="2d039-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d039-132">id</span><span class="sxs-lookup"><span data-stu-id="2d039-132">id</span></span>|<span data-ttu-id="2d039-133">String</span><span class="sxs-lookup"><span data-stu-id="2d039-133">String</span></span>|<span data-ttu-id="2d039-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2d039-134">Not yet documented</span></span>|
|<span data-ttu-id="2d039-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="2d039-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="2d039-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d039-136">DateTimeOffset</span></span>|<span data-ttu-id="2d039-137">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="2d039-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="2d039-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="2d039-138">partnerState</span></span>|[<span data-ttu-id="2d039-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="2d039-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="2d039-140">数据同步此帐户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="2d039-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="2d039-141">可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="2d039-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="2d039-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="2d039-142">androidEnabled</span></span>|<span data-ttu-id="2d039-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d039-143">Boolean</span></span>|<span data-ttu-id="2d039-144">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="2d039-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2d039-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="2d039-145">iosEnabled</span></span>|<span data-ttu-id="2d039-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d039-146">Boolean</span></span>|<span data-ttu-id="2d039-147">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="2d039-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2d039-148">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2d039-148">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2d039-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d039-149">Boolean</span></span>|<span data-ttu-id="2d039-150">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="2d039-150">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2d039-151">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2d039-151">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2d039-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d039-152">Boolean</span></span>|<span data-ttu-id="2d039-153">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="2d039-153">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2d039-154">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="2d039-154">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="2d039-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d039-155">Boolean</span></span>|<span data-ttu-id="2d039-156">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="2d039-156">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="2d039-157">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="2d039-157">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="2d039-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2d039-158">Int32</span></span>|<span data-ttu-id="2d039-159">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="2d039-159">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="2d039-160">响应</span><span class="sxs-lookup"><span data-stu-id="2d039-160">Response</span></span>
<span data-ttu-id="2d039-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d039-161">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d039-162">示例</span><span class="sxs-lookup"><span data-stu-id="2d039-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d039-163">请求</span><span class="sxs-lookup"><span data-stu-id="2d039-163">Request</span></span>
<span data-ttu-id="2d039-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d039-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
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

### <a name="response"></a><span data-ttu-id="2d039-165">响应</span><span class="sxs-lookup"><span data-stu-id="2d039-165">Response</span></span>
<span data-ttu-id="2d039-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d039-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




