---
title: 创建 mobileAppIntentAndState
description: 创建新的 mobileAppIntentAndState 对象。
author: tfitzmac
ms.openlocfilehash: 590cbb01e8b1f41ce1a1c43be7c3a97872ea737a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308699"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="3c9f0-103">创建 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="3c9f0-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="3c9f0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c9f0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c9f0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c9f0-107">创建新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-107">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c9f0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c9f0-108">Prerequisites</span></span>
<span data-ttu-id="3c9f0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3c9f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c9f0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c9f0-111">Permission type</span></span>|<span data-ttu-id="3c9f0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c9f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c9f0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c9f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c9f0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c9f0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3c9f0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c9f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c9f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-116">Not supported.</span></span>|
|<span data-ttu-id="3c9f0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c9f0-117">Application</span></span>|<span data-ttu-id="3c9f0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c9f0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c9f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="3c9f0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c9f0-120">Request headers</span></span>
|<span data-ttu-id="3c9f0-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c9f0-121">Header</span></span>|<span data-ttu-id="3c9f0-122">值</span><span class="sxs-lookup"><span data-stu-id="3c9f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c9f0-123">授权</span><span class="sxs-lookup"><span data-stu-id="3c9f0-123">Authorization</span></span>|<span data-ttu-id="3c9f0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c9f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c9f0-125">Accept</span></span>|<span data-ttu-id="3c9f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c9f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c9f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c9f0-127">Request body</span></span>
<span data-ttu-id="3c9f0-128">在请求正文中，提供 mobileAppIntentAndState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-128">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="3c9f0-129">下表显示时创建 mobileAppIntentAndState 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-129">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="3c9f0-130">属性</span><span class="sxs-lookup"><span data-stu-id="3c9f0-130">Property</span></span>|<span data-ttu-id="3c9f0-131">类型</span><span class="sxs-lookup"><span data-stu-id="3c9f0-131">Type</span></span>|<span data-ttu-id="3c9f0-132">说明</span><span class="sxs-lookup"><span data-stu-id="3c9f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c9f0-133">id</span><span class="sxs-lookup"><span data-stu-id="3c9f0-133">id</span></span>|<span data-ttu-id="3c9f0-134">String</span><span class="sxs-lookup"><span data-stu-id="3c9f0-134">String</span></span>|<span data-ttu-id="3c9f0-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="3c9f0-135">UUID for the object</span></span>|
|<span data-ttu-id="3c9f0-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3c9f0-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="3c9f0-137">String</span><span class="sxs-lookup"><span data-stu-id="3c9f0-137">String</span></span>|<span data-ttu-id="3c9f0-138">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="3c9f0-139">userId</span><span class="sxs-lookup"><span data-stu-id="3c9f0-139">userId</span></span>|<span data-ttu-id="3c9f0-140">String</span><span class="sxs-lookup"><span data-stu-id="3c9f0-140">String</span></span>|<span data-ttu-id="3c9f0-141">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="3c9f0-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="3c9f0-142">mobileAppList</span></span>|<span data-ttu-id="3c9f0-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9f0-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="3c9f0-144">负载方法和租户的状态的列表。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="3c9f0-145">响应</span><span class="sxs-lookup"><span data-stu-id="3c9f0-145">Response</span></span>
<span data-ttu-id="3c9f0-146">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-146">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c9f0-147">示例</span><span class="sxs-lookup"><span data-stu-id="3c9f0-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c9f0-148">请求</span><span class="sxs-lookup"><span data-stu-id="3c9f0-148">Request</span></span>
<span data-ttu-id="3c9f0-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3c9f0-150">响应</span><span class="sxs-lookup"><span data-stu-id="3c9f0-150">Response</span></span>
<span data-ttu-id="3c9f0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c9f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





