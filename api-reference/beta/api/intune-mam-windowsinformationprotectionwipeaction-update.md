---
title: 更新 windowsInformationProtectionWipeAction
description: 更新 windowsInformationProtectionWipeAction 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f82f7ba6d541f1a4a20721e7395b981659f5427
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462795"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="feb4c-103">更新 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="feb4c-103">Update windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="feb4c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="feb4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="feb4c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="feb4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feb4c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="feb4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb4c-107">更新[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="feb4c-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feb4c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="feb4c-108">Prerequisites</span></span>
<span data-ttu-id="feb4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="feb4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feb4c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="feb4c-111">Permission type</span></span>|<span data-ttu-id="feb4c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="feb4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feb4c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="feb4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="feb4c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb4c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="feb4c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="feb4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feb4c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="feb4c-116">Not supported.</span></span>|
|<span data-ttu-id="feb4c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="feb4c-117">Application</span></span>|<span data-ttu-id="feb4c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb4c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="feb4c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="feb4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="feb4c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="feb4c-120">Request headers</span></span>
|<span data-ttu-id="feb4c-121">标头</span><span class="sxs-lookup"><span data-stu-id="feb4c-121">Header</span></span>|<span data-ttu-id="feb4c-122">值</span><span class="sxs-lookup"><span data-stu-id="feb4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feb4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="feb4c-123">Authorization</span></span>|<span data-ttu-id="feb4c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="feb4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feb4c-125">接受</span><span class="sxs-lookup"><span data-stu-id="feb4c-125">Accept</span></span>|<span data-ttu-id="feb4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="feb4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feb4c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="feb4c-127">Request body</span></span>
<span data-ttu-id="feb4c-128">在请求正文中，提供[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="feb4c-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="feb4c-129">下表显示创建[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="feb4c-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="feb4c-130">属性</span><span class="sxs-lookup"><span data-stu-id="feb4c-130">Property</span></span>|<span data-ttu-id="feb4c-131">类型</span><span class="sxs-lookup"><span data-stu-id="feb4c-131">Type</span></span>|<span data-ttu-id="feb4c-132">说明</span><span class="sxs-lookup"><span data-stu-id="feb4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb4c-133">id</span><span class="sxs-lookup"><span data-stu-id="feb4c-133">id</span></span>|<span data-ttu-id="feb4c-134">String</span><span class="sxs-lookup"><span data-stu-id="feb4c-134">String</span></span>|<span data-ttu-id="feb4c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="feb4c-135">Key of the entity.</span></span>|
|<span data-ttu-id="feb4c-136">status</span><span class="sxs-lookup"><span data-stu-id="feb4c-136">status</span></span>|[<span data-ttu-id="feb4c-137">actionState</span><span class="sxs-lookup"><span data-stu-id="feb4c-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="feb4c-138">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="feb4c-138">Wipe action status.</span></span> <span data-ttu-id="feb4c-139">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="feb4c-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="feb4c-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="feb4c-140">targetedUserId</span></span>|<span data-ttu-id="feb4c-141">String</span><span class="sxs-lookup"><span data-stu-id="feb4c-141">String</span></span>|<span data-ttu-id="feb4c-142">此擦除操作针对的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="feb4c-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="feb4c-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="feb4c-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="feb4c-144">String</span><span class="sxs-lookup"><span data-stu-id="feb4c-144">String</span></span>|<span data-ttu-id="feb4c-145">此擦除操作针对的 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="feb4c-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="feb4c-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="feb4c-146">targetedDeviceName</span></span>|<span data-ttu-id="feb4c-147">String</span><span class="sxs-lookup"><span data-stu-id="feb4c-147">String</span></span>|<span data-ttu-id="feb4c-148">目标设备名称。</span><span class="sxs-lookup"><span data-stu-id="feb4c-148">Targeted device name.</span></span>|
|<span data-ttu-id="feb4c-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="feb4c-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="feb4c-150">String</span><span class="sxs-lookup"><span data-stu-id="feb4c-150">String</span></span>|<span data-ttu-id="feb4c-151">目标设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="feb4c-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="feb4c-152">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="feb4c-152">lastCheckInDateTime</span></span>|<span data-ttu-id="feb4c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feb4c-153">DateTimeOffset</span></span>|<span data-ttu-id="feb4c-154">此擦除操作所针对的设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="feb4c-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="feb4c-155">响应</span><span class="sxs-lookup"><span data-stu-id="feb4c-155">Response</span></span>
<span data-ttu-id="feb4c-156">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="feb4c-156">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feb4c-157">示例</span><span class="sxs-lookup"><span data-stu-id="feb4c-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="feb4c-158">请求</span><span class="sxs-lookup"><span data-stu-id="feb4c-158">Request</span></span>
<span data-ttu-id="feb4c-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="feb4c-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="feb4c-160">响应</span><span class="sxs-lookup"><span data-stu-id="feb4c-160">Response</span></span>
<span data-ttu-id="feb4c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="feb4c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





