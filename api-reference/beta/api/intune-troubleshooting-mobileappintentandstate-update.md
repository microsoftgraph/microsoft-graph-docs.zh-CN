---
title: 更新 mobileAppIntentAndState
description: 更新 mobileAppIntentAndState 对象的属性。
author: tfitzmac
ms.openlocfilehash: d219e6d9d146f71c4979973e7f6510010fe2fa92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303183"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="789ae-103">更新 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="789ae-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="789ae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="789ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="789ae-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="789ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="789ae-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="789ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="789ae-107">更新[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="789ae-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="789ae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="789ae-108">Prerequisites</span></span>
<span data-ttu-id="789ae-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="789ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="789ae-111">Permission type</span></span>|<span data-ttu-id="789ae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="789ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="789ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="789ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="789ae-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789ae-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="789ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="789ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="789ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="789ae-116">Not supported.</span></span>|
|<span data-ttu-id="789ae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="789ae-117">Application</span></span>|<span data-ttu-id="789ae-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="789ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="789ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="789ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="789ae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="789ae-120">Request headers</span></span>
|<span data-ttu-id="789ae-121">标头</span><span class="sxs-lookup"><span data-stu-id="789ae-121">Header</span></span>|<span data-ttu-id="789ae-122">值</span><span class="sxs-lookup"><span data-stu-id="789ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="789ae-123">授权</span><span class="sxs-lookup"><span data-stu-id="789ae-123">Authorization</span></span>|<span data-ttu-id="789ae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="789ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="789ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="789ae-125">Accept</span></span>|<span data-ttu-id="789ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="789ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="789ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="789ae-127">Request body</span></span>
<span data-ttu-id="789ae-128">在请求正文中，提供[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="789ae-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="789ae-129">下表显示时创建[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="789ae-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="789ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="789ae-130">Property</span></span>|<span data-ttu-id="789ae-131">类型</span><span class="sxs-lookup"><span data-stu-id="789ae-131">Type</span></span>|<span data-ttu-id="789ae-132">说明</span><span class="sxs-lookup"><span data-stu-id="789ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="789ae-133">id</span><span class="sxs-lookup"><span data-stu-id="789ae-133">id</span></span>|<span data-ttu-id="789ae-134">String</span><span class="sxs-lookup"><span data-stu-id="789ae-134">String</span></span>|<span data-ttu-id="789ae-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="789ae-135">UUID for the object</span></span>|
|<span data-ttu-id="789ae-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="789ae-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="789ae-137">String</span><span class="sxs-lookup"><span data-stu-id="789ae-137">String</span></span>|<span data-ttu-id="789ae-138">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="789ae-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="789ae-139">userId</span><span class="sxs-lookup"><span data-stu-id="789ae-139">userId</span></span>|<span data-ttu-id="789ae-140">String</span><span class="sxs-lookup"><span data-stu-id="789ae-140">String</span></span>|<span data-ttu-id="789ae-141">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="789ae-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="789ae-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="789ae-142">mobileAppList</span></span>|<span data-ttu-id="789ae-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="789ae-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="789ae-144">负载方法和租户的状态的列表。</span><span class="sxs-lookup"><span data-stu-id="789ae-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="789ae-145">响应</span><span class="sxs-lookup"><span data-stu-id="789ae-145">Response</span></span>
<span data-ttu-id="789ae-146">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="789ae-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="789ae-147">示例</span><span class="sxs-lookup"><span data-stu-id="789ae-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="789ae-148">请求</span><span class="sxs-lookup"><span data-stu-id="789ae-148">Request</span></span>
<span data-ttu-id="789ae-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="789ae-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
Content-type: application/json
Content-length: 769

{
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

### <a name="response"></a><span data-ttu-id="789ae-150">响应</span><span class="sxs-lookup"><span data-stu-id="789ae-150">Response</span></span>
<span data-ttu-id="789ae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="789ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





