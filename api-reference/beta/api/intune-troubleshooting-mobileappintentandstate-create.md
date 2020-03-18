---
title: 创建 mobileAppIntentAndState
description: 创建新的 mobileAppIntentAndState 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6b5132675f09da3b26ffca6e51893ab64afed43
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800121"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="310f3-103">创建 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="310f3-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="310f3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="310f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="310f3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="310f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="310f3-106">创建新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="310f3-106">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="310f3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="310f3-107">Prerequisites</span></span>
<span data-ttu-id="310f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="310f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="310f3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="310f3-110">Permission type</span></span>|<span data-ttu-id="310f3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="310f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="310f3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="310f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="310f3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310f3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="310f3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="310f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="310f3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="310f3-115">Not supported.</span></span>|
|<span data-ttu-id="310f3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="310f3-116">Application</span></span>|<span data-ttu-id="310f3-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310f3-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="310f3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="310f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="310f3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="310f3-119">Request headers</span></span>
|<span data-ttu-id="310f3-120">标头</span><span class="sxs-lookup"><span data-stu-id="310f3-120">Header</span></span>|<span data-ttu-id="310f3-121">值</span><span class="sxs-lookup"><span data-stu-id="310f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="310f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="310f3-122">Authorization</span></span>|<span data-ttu-id="310f3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="310f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="310f3-124">接受</span><span class="sxs-lookup"><span data-stu-id="310f3-124">Accept</span></span>|<span data-ttu-id="310f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="310f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="310f3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="310f3-126">Request body</span></span>
<span data-ttu-id="310f3-127">在请求正文中，提供 mobileAppIntentAndState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="310f3-127">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="310f3-128">下表显示创建 mobileAppIntentAndState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="310f3-128">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="310f3-129">属性</span><span class="sxs-lookup"><span data-stu-id="310f3-129">Property</span></span>|<span data-ttu-id="310f3-130">类型</span><span class="sxs-lookup"><span data-stu-id="310f3-130">Type</span></span>|<span data-ttu-id="310f3-131">说明</span><span class="sxs-lookup"><span data-stu-id="310f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="310f3-132">id</span><span class="sxs-lookup"><span data-stu-id="310f3-132">id</span></span>|<span data-ttu-id="310f3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="310f3-133">String</span></span>|<span data-ttu-id="310f3-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="310f3-134">UUID for the object</span></span>|
|<span data-ttu-id="310f3-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="310f3-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="310f3-136">String</span><span class="sxs-lookup"><span data-stu-id="310f3-136">String</span></span>|<span data-ttu-id="310f3-137">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="310f3-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="310f3-138">userId</span><span class="sxs-lookup"><span data-stu-id="310f3-138">userId</span></span>|<span data-ttu-id="310f3-139">String</span><span class="sxs-lookup"><span data-stu-id="310f3-139">String</span></span>|<span data-ttu-id="310f3-140">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="310f3-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="310f3-141">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="310f3-141">mobileAppList</span></span>|<span data-ttu-id="310f3-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="310f3-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="310f3-143">租户的有效负载意图和状态列表。</span><span class="sxs-lookup"><span data-stu-id="310f3-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="310f3-144">响应</span><span class="sxs-lookup"><span data-stu-id="310f3-144">Response</span></span>
<span data-ttu-id="310f3-145">如果成功，此方法在响应`201 Created`正文中返回响应代码和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="310f3-145">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="310f3-146">示例</span><span class="sxs-lookup"><span data-stu-id="310f3-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="310f3-147">请求</span><span class="sxs-lookup"><span data-stu-id="310f3-147">Request</span></span>
<span data-ttu-id="310f3-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="310f3-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="310f3-149">响应</span><span class="sxs-lookup"><span data-stu-id="310f3-149">Response</span></span>
<span data-ttu-id="310f3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="310f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```




