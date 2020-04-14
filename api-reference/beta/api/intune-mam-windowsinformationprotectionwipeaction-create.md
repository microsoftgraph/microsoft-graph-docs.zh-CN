---
title: 创建 windowsInformationProtectionWipeAction
description: 创建新的 windowsInformationProtectionWipeAction 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18174f52cc5adec826ff497797f92ec7ce0516c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440792"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="88dfe-103">创建 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="88dfe-103">Create windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="88dfe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88dfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88dfe-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88dfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88dfe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88dfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88dfe-107">创建新的[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88dfe-107">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88dfe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88dfe-108">Prerequisites</span></span>
<span data-ttu-id="88dfe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88dfe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88dfe-111">Permission type</span></span>|<span data-ttu-id="88dfe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88dfe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88dfe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88dfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88dfe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88dfe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="88dfe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88dfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88dfe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88dfe-116">Not supported.</span></span>|
|<span data-ttu-id="88dfe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88dfe-117">Application</span></span>|<span data-ttu-id="88dfe-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88dfe-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88dfe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88dfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="88dfe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88dfe-120">Request headers</span></span>
|<span data-ttu-id="88dfe-121">标头</span><span class="sxs-lookup"><span data-stu-id="88dfe-121">Header</span></span>|<span data-ttu-id="88dfe-122">值</span><span class="sxs-lookup"><span data-stu-id="88dfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88dfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88dfe-123">Authorization</span></span>|<span data-ttu-id="88dfe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88dfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88dfe-125">接受</span><span class="sxs-lookup"><span data-stu-id="88dfe-125">Accept</span></span>|<span data-ttu-id="88dfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88dfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88dfe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88dfe-127">Request body</span></span>
<span data-ttu-id="88dfe-128">在请求正文中，提供 windowsInformationProtectionWipeAction 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88dfe-128">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="88dfe-129">下表显示创建 windowsInformationProtectionWipeAction 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88dfe-129">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="88dfe-130">属性</span><span class="sxs-lookup"><span data-stu-id="88dfe-130">Property</span></span>|<span data-ttu-id="88dfe-131">类型</span><span class="sxs-lookup"><span data-stu-id="88dfe-131">Type</span></span>|<span data-ttu-id="88dfe-132">说明</span><span class="sxs-lookup"><span data-stu-id="88dfe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dfe-133">id</span><span class="sxs-lookup"><span data-stu-id="88dfe-133">id</span></span>|<span data-ttu-id="88dfe-134">String</span><span class="sxs-lookup"><span data-stu-id="88dfe-134">String</span></span>|<span data-ttu-id="88dfe-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88dfe-135">Key of the entity.</span></span>|
|<span data-ttu-id="88dfe-136">状态</span><span class="sxs-lookup"><span data-stu-id="88dfe-136">status</span></span>|[<span data-ttu-id="88dfe-137">actionState</span><span class="sxs-lookup"><span data-stu-id="88dfe-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="88dfe-138">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="88dfe-138">Wipe action status.</span></span> <span data-ttu-id="88dfe-139">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="88dfe-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="88dfe-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="88dfe-140">targetedUserId</span></span>|<span data-ttu-id="88dfe-141">String</span><span class="sxs-lookup"><span data-stu-id="88dfe-141">String</span></span>|<span data-ttu-id="88dfe-142">此擦除操作针对的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="88dfe-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="88dfe-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="88dfe-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="88dfe-144">String</span><span class="sxs-lookup"><span data-stu-id="88dfe-144">String</span></span>|<span data-ttu-id="88dfe-145">此擦除操作针对的 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="88dfe-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="88dfe-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="88dfe-146">targetedDeviceName</span></span>|<span data-ttu-id="88dfe-147">String</span><span class="sxs-lookup"><span data-stu-id="88dfe-147">String</span></span>|<span data-ttu-id="88dfe-148">目标设备名称。</span><span class="sxs-lookup"><span data-stu-id="88dfe-148">Targeted device name.</span></span>|
|<span data-ttu-id="88dfe-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="88dfe-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="88dfe-150">String</span><span class="sxs-lookup"><span data-stu-id="88dfe-150">String</span></span>|<span data-ttu-id="88dfe-151">目标设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="88dfe-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="88dfe-152">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="88dfe-152">lastCheckInDateTime</span></span>|<span data-ttu-id="88dfe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88dfe-153">DateTimeOffset</span></span>|<span data-ttu-id="88dfe-154">此擦除操作所针对的设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="88dfe-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="88dfe-155">响应</span><span class="sxs-lookup"><span data-stu-id="88dfe-155">Response</span></span>
<span data-ttu-id="88dfe-156">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88dfe-156">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88dfe-157">示例</span><span class="sxs-lookup"><span data-stu-id="88dfe-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="88dfe-158">请求</span><span class="sxs-lookup"><span data-stu-id="88dfe-158">Request</span></span>
<span data-ttu-id="88dfe-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88dfe-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
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

### <a name="response"></a><span data-ttu-id="88dfe-160">响应</span><span class="sxs-lookup"><span data-stu-id="88dfe-160">Response</span></span>
<span data-ttu-id="88dfe-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88dfe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



