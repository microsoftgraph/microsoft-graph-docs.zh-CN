---
title: 更新 mobileAppTroubleshootingEvent
description: 更新 mobileAppTroubleshootingEvent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ec0c30cc2c37e65fa0a6adebf0bd3a171530640d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940069"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="4c0d9-103">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4c0d9-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="4c0d9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c0d9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c0d9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c0d9-107">更新[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c0d9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c0d9-108">Prerequisites</span></span>
<span data-ttu-id="4c0d9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4c0d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c0d9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c0d9-111">Permission type</span></span>|<span data-ttu-id="4c0d9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c0d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c0d9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c0d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c0d9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c0d9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4c0d9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c0d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c0d9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-116">Not supported.</span></span>|
|<span data-ttu-id="4c0d9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c0d9-117">Application</span></span>|<span data-ttu-id="4c0d9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c0d9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c0d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="4c0d9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c0d9-120">Request headers</span></span>
|<span data-ttu-id="4c0d9-121">标头</span><span class="sxs-lookup"><span data-stu-id="4c0d9-121">Header</span></span>|<span data-ttu-id="4c0d9-122">值</span><span class="sxs-lookup"><span data-stu-id="4c0d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c0d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c0d9-123">Authorization</span></span>|<span data-ttu-id="4c0d9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c0d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c0d9-125">Accept</span></span>|<span data-ttu-id="4c0d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c0d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c0d9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c0d9-127">Request body</span></span>
<span data-ttu-id="4c0d9-128">在请求正文中，提供[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-128">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="4c0d9-129">下表显示时创建[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-129">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="4c0d9-130">属性</span><span class="sxs-lookup"><span data-stu-id="4c0d9-130">Property</span></span>|<span data-ttu-id="4c0d9-131">类型</span><span class="sxs-lookup"><span data-stu-id="4c0d9-131">Type</span></span>|<span data-ttu-id="4c0d9-132">说明</span><span class="sxs-lookup"><span data-stu-id="4c0d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c0d9-133">id</span><span class="sxs-lookup"><span data-stu-id="4c0d9-133">id</span></span>|<span data-ttu-id="4c0d9-134">String</span><span class="sxs-lookup"><span data-stu-id="4c0d9-134">String</span></span>|<span data-ttu-id="4c0d9-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4c0d9-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4c0d9-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4c0d9-136">eventDateTime</span></span>|<span data-ttu-id="4c0d9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c0d9-137">DateTimeOffset</span></span>|<span data-ttu-id="4c0d9-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-138">Time when the event occurred .</span></span> <span data-ttu-id="4c0d9-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4c0d9-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4c0d9-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="4c0d9-140">correlationId</span></span>|<span data-ttu-id="4c0d9-141">String</span><span class="sxs-lookup"><span data-stu-id="4c0d9-141">String</span></span>|<span data-ttu-id="4c0d9-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="4c0d9-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4c0d9-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4c0d9-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4c0d9-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="4c0d9-145">String</span><span class="sxs-lookup"><span data-stu-id="4c0d9-145">String</span></span>|<span data-ttu-id="4c0d9-146">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="4c0d9-147">userId</span><span class="sxs-lookup"><span data-stu-id="4c0d9-147">userId</span></span>|<span data-ttu-id="4c0d9-148">String</span><span class="sxs-lookup"><span data-stu-id="4c0d9-148">String</span></span>|<span data-ttu-id="4c0d9-149">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="4c0d9-150">applicationId</span><span class="sxs-lookup"><span data-stu-id="4c0d9-150">applicationId</span></span>|<span data-ttu-id="4c0d9-151">String</span><span class="sxs-lookup"><span data-stu-id="4c0d9-151">String</span></span>|<span data-ttu-id="4c0d9-152">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-152">Intune application identifier.</span></span>|
|<span data-ttu-id="4c0d9-153">历史记录</span><span class="sxs-lookup"><span data-stu-id="4c0d9-153">history</span></span>|<span data-ttu-id="4c0d9-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="4c0d9-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="4c0d9-155">疑难解答历史记录项 Intune 移动应用程序</span><span class="sxs-lookup"><span data-stu-id="4c0d9-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="4c0d9-156">响应</span><span class="sxs-lookup"><span data-stu-id="4c0d9-156">Response</span></span>
<span data-ttu-id="4c0d9-157">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-157">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c0d9-158">示例</span><span class="sxs-lookup"><span data-stu-id="4c0d9-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c0d9-159">请求</span><span class="sxs-lookup"><span data-stu-id="4c0d9-159">Request</span></span>
<span data-ttu-id="4c0d9-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 421

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4c0d9-161">响应</span><span class="sxs-lookup"><span data-stu-id="4c0d9-161">Response</span></span>
<span data-ttu-id="4c0d9-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c0d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 538

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```





