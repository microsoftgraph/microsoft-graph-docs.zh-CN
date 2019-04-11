---
title: 更新 windowsInformationProtectionWipeAction
description: 更新 windowsInformationProtectionWipeAction 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e59eeb987e678764adcd5f4378f6bfdc5b4907e0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777604"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="65eb1-103">更新 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="65eb1-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="65eb1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65eb1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65eb1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65eb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65eb1-106">更新[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65eb1-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65eb1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="65eb1-107">Prerequisites</span></span>
<span data-ttu-id="65eb1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65eb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65eb1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="65eb1-110">Permission type</span></span>|<span data-ttu-id="65eb1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65eb1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65eb1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65eb1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65eb1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65eb1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65eb1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65eb1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65eb1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65eb1-115">Not supported.</span></span>|
|<span data-ttu-id="65eb1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65eb1-116">Application</span></span>|<span data-ttu-id="65eb1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="65eb1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65eb1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65eb1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="65eb1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65eb1-119">Request headers</span></span>
|<span data-ttu-id="65eb1-120">标头</span><span class="sxs-lookup"><span data-stu-id="65eb1-120">Header</span></span>|<span data-ttu-id="65eb1-121">值</span><span class="sxs-lookup"><span data-stu-id="65eb1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65eb1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65eb1-122">Authorization</span></span>|<span data-ttu-id="65eb1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65eb1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65eb1-124">接受</span><span class="sxs-lookup"><span data-stu-id="65eb1-124">Accept</span></span>|<span data-ttu-id="65eb1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65eb1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65eb1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65eb1-126">Request body</span></span>
<span data-ttu-id="65eb1-127">在请求正文中, 提供[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65eb1-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="65eb1-128">下表显示创建[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65eb1-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="65eb1-129">属性</span><span class="sxs-lookup"><span data-stu-id="65eb1-129">Property</span></span>|<span data-ttu-id="65eb1-130">类型</span><span class="sxs-lookup"><span data-stu-id="65eb1-130">Type</span></span>|<span data-ttu-id="65eb1-131">说明</span><span class="sxs-lookup"><span data-stu-id="65eb1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65eb1-132">id</span><span class="sxs-lookup"><span data-stu-id="65eb1-132">id</span></span>|<span data-ttu-id="65eb1-133">String</span><span class="sxs-lookup"><span data-stu-id="65eb1-133">String</span></span>|<span data-ttu-id="65eb1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65eb1-134">Key of the entity.</span></span>|
|<span data-ttu-id="65eb1-135">status</span><span class="sxs-lookup"><span data-stu-id="65eb1-135">status</span></span>|[<span data-ttu-id="65eb1-136">actionState</span><span class="sxs-lookup"><span data-stu-id="65eb1-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="65eb1-137">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="65eb1-137">Wipe action status.</span></span> <span data-ttu-id="65eb1-138">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="65eb1-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="65eb1-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="65eb1-139">targetedUserId</span></span>|<span data-ttu-id="65eb1-140">String</span><span class="sxs-lookup"><span data-stu-id="65eb1-140">String</span></span>|<span data-ttu-id="65eb1-141">此擦除操作针对的用户 id。</span><span class="sxs-lookup"><span data-stu-id="65eb1-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="65eb1-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="65eb1-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="65eb1-143">String</span><span class="sxs-lookup"><span data-stu-id="65eb1-143">String</span></span>|<span data-ttu-id="65eb1-144">此擦除操作针对的 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="65eb1-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="65eb1-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="65eb1-145">targetedDeviceName</span></span>|<span data-ttu-id="65eb1-146">String</span><span class="sxs-lookup"><span data-stu-id="65eb1-146">String</span></span>|<span data-ttu-id="65eb1-147">目标设备名称。</span><span class="sxs-lookup"><span data-stu-id="65eb1-147">Targeted device name.</span></span>|
|<span data-ttu-id="65eb1-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="65eb1-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="65eb1-149">String</span><span class="sxs-lookup"><span data-stu-id="65eb1-149">String</span></span>|<span data-ttu-id="65eb1-150">目标设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="65eb1-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="65eb1-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="65eb1-151">lastCheckInDateTime</span></span>|<span data-ttu-id="65eb1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65eb1-152">DateTimeOffset</span></span>|<span data-ttu-id="65eb1-153">此擦除操作所针对的设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="65eb1-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="65eb1-154">响应</span><span class="sxs-lookup"><span data-stu-id="65eb1-154">Response</span></span>
<span data-ttu-id="65eb1-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65eb1-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65eb1-156">示例</span><span class="sxs-lookup"><span data-stu-id="65eb1-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="65eb1-157">请求</span><span class="sxs-lookup"><span data-stu-id="65eb1-157">Request</span></span>
<span data-ttu-id="65eb1-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65eb1-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="65eb1-159">响应</span><span class="sxs-lookup"><span data-stu-id="65eb1-159">Response</span></span>
<span data-ttu-id="65eb1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65eb1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```





