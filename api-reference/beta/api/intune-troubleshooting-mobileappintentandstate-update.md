---
title: 更新 mobileAppIntentAndState
description: 更新 mobileAppIntentAndState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65a2076469d01891f889d1b4df11ba8ad1e2b445
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141489"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="c0fa6-103">更新 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c0fa6-103">Update mobileAppIntentAndState</span></span>

<span data-ttu-id="c0fa6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0fa6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0fa6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0fa6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0fa6-107">更新 [mobileAppIntentAndState 对象](../resources/intune-troubleshooting-mobileappintentandstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0fa6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0fa6-108">Prerequisites</span></span>
<span data-ttu-id="c0fa6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0fa6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0fa6-111">Permission type</span></span>|<span data-ttu-id="c0fa6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0fa6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0fa6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0fa6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fa6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c0fa6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0fa6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-116">Not supported.</span></span>|
|<span data-ttu-id="c0fa6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0fa6-117">Application</span></span>|<span data-ttu-id="c0fa6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fa6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0fa6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0fa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c0fa6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0fa6-120">Request headers</span></span>
|<span data-ttu-id="c0fa6-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0fa6-121">Header</span></span>|<span data-ttu-id="c0fa6-122">值</span><span class="sxs-lookup"><span data-stu-id="c0fa6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0fa6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0fa6-123">Authorization</span></span>|<span data-ttu-id="c0fa6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0fa6-125">接受</span><span class="sxs-lookup"><span data-stu-id="c0fa6-125">Accept</span></span>|<span data-ttu-id="c0fa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0fa6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0fa6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0fa6-127">Request body</span></span>
<span data-ttu-id="c0fa6-128">在请求正文中，提供 [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="c0fa6-129">下表显示创建 [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="c0fa6-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0fa6-130">Property</span></span>|<span data-ttu-id="c0fa6-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0fa6-131">Type</span></span>|<span data-ttu-id="c0fa6-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0fa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0fa6-133">id</span><span class="sxs-lookup"><span data-stu-id="c0fa6-133">id</span></span>|<span data-ttu-id="c0fa6-134">String</span><span class="sxs-lookup"><span data-stu-id="c0fa6-134">String</span></span>|<span data-ttu-id="c0fa6-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="c0fa6-135">UUID for the object</span></span>|
|<span data-ttu-id="c0fa6-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c0fa6-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="c0fa6-137">String</span><span class="sxs-lookup"><span data-stu-id="c0fa6-137">String</span></span>|<span data-ttu-id="c0fa6-138">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c0fa6-139">userId</span><span class="sxs-lookup"><span data-stu-id="c0fa6-139">userId</span></span>|<span data-ttu-id="c0fa6-140">String</span><span class="sxs-lookup"><span data-stu-id="c0fa6-140">String</span></span>|<span data-ttu-id="c0fa6-141">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c0fa6-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="c0fa6-142">mobileAppList</span></span>|<span data-ttu-id="c0fa6-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0fa6-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="c0fa6-144">租户的有效负载意图和状态列表。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="c0fa6-145">响应</span><span class="sxs-lookup"><span data-stu-id="c0fa6-145">Response</span></span>
<span data-ttu-id="c0fa6-146">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0fa6-147">示例</span><span class="sxs-lookup"><span data-stu-id="c0fa6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0fa6-148">请求</span><span class="sxs-lookup"><span data-stu-id="c0fa6-148">Request</span></span>
<span data-ttu-id="c0fa6-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
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

### <a name="response"></a><span data-ttu-id="c0fa6-150">响应</span><span class="sxs-lookup"><span data-stu-id="c0fa6-150">Response</span></span>
<span data-ttu-id="c0fa6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0fa6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




