---
title: 更新 iosUpdateConfiguration
description: 更新 iosUpdateConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfc9be70f26b9d4ed58dfca1274a828237ebb473
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982223"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="d8e82-103">更新 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8e82-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="d8e82-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d8e82-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8e82-105">更新 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8e82-105">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8e82-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8e82-106">Prerequisites</span></span>
<span data-ttu-id="d8e82-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d8e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8e82-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8e82-109">Permission type</span></span>|<span data-ttu-id="d8e82-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8e82-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8e82-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8e82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8e82-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e82-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8e82-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8e82-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8e82-114">Not supported.</span></span>|
|<span data-ttu-id="d8e82-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8e82-115">Application</span></span>|<span data-ttu-id="d8e82-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8e82-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e82-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8e82-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8e82-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8e82-118">Request headers</span></span>
|<span data-ttu-id="d8e82-119">标头</span><span class="sxs-lookup"><span data-stu-id="d8e82-119">Header</span></span>|<span data-ttu-id="d8e82-120">值</span><span class="sxs-lookup"><span data-stu-id="d8e82-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8e82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8e82-121">Authorization</span></span>|<span data-ttu-id="d8e82-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8e82-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8e82-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d8e82-123">Accept</span></span>|<span data-ttu-id="d8e82-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d8e82-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e82-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8e82-125">Request body</span></span>
<span data-ttu-id="d8e82-126">在请求正文中，提供 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8e82-126">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="d8e82-127">下表显示创建 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8e82-127">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="d8e82-128">属性</span><span class="sxs-lookup"><span data-stu-id="d8e82-128">Property</span></span>|<span data-ttu-id="d8e82-129">类型</span><span class="sxs-lookup"><span data-stu-id="d8e82-129">Type</span></span>|<span data-ttu-id="d8e82-130">说明</span><span class="sxs-lookup"><span data-stu-id="d8e82-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e82-131">id</span><span class="sxs-lookup"><span data-stu-id="d8e82-131">id</span></span>|<span data-ttu-id="d8e82-132">String</span><span class="sxs-lookup"><span data-stu-id="d8e82-132">String</span></span>|<span data-ttu-id="d8e82-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8e82-133">Key of the entity.</span></span> <span data-ttu-id="d8e82-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e82-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e82-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e82-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d8e82-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e82-136">DateTimeOffset</span></span>|<span data-ttu-id="d8e82-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8e82-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d8e82-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e82-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e82-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e82-139">createdDateTime</span></span>|<span data-ttu-id="d8e82-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e82-140">DateTimeOffset</span></span>|<span data-ttu-id="d8e82-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8e82-141">DateTime the object was created.</span></span> <span data-ttu-id="d8e82-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e82-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e82-143">description</span><span class="sxs-lookup"><span data-stu-id="d8e82-143">description</span></span>|<span data-ttu-id="d8e82-144">String</span><span class="sxs-lookup"><span data-stu-id="d8e82-144">String</span></span>|<span data-ttu-id="d8e82-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d8e82-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8e82-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e82-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e82-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d8e82-147">displayName</span></span>|<span data-ttu-id="d8e82-148">String</span><span class="sxs-lookup"><span data-stu-id="d8e82-148">String</span></span>|<span data-ttu-id="d8e82-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d8e82-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8e82-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e82-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e82-151">version</span><span class="sxs-lookup"><span data-stu-id="d8e82-151">version</span></span>|<span data-ttu-id="d8e82-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e82-152">Int32</span></span>|<span data-ttu-id="d8e82-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d8e82-153">Version of the device configuration.</span></span> <span data-ttu-id="d8e82-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e82-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e82-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d8e82-155">activeHoursStart</span></span>|<span data-ttu-id="d8e82-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d8e82-156">TimeOfDay</span></span>|<span data-ttu-id="d8e82-157">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="d8e82-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="d8e82-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d8e82-158">activeHoursEnd</span></span>|<span data-ttu-id="d8e82-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d8e82-159">TimeOfDay</span></span>|<span data-ttu-id="d8e82-160">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="d8e82-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="d8e82-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="d8e82-161">scheduledInstallDays</span></span>|<span data-ttu-id="d8e82-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="d8e82-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="d8e82-163">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="d8e82-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="d8e82-164">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="d8e82-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="d8e82-165">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="d8e82-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d8e82-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="d8e82-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="d8e82-167">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e82-167">Int32</span></span>|<span data-ttu-id="d8e82-168">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="d8e82-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="d8e82-169">响应</span><span class="sxs-lookup"><span data-stu-id="d8e82-169">Response</span></span>
<span data-ttu-id="d8e82-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8e82-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e82-171">示例</span><span class="sxs-lookup"><span data-stu-id="d8e82-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8e82-172">请求</span><span class="sxs-lookup"><span data-stu-id="d8e82-172">Request</span></span>
<span data-ttu-id="d8e82-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8e82-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="d8e82-174">响应</span><span class="sxs-lookup"><span data-stu-id="d8e82-174">Response</span></span>
<span data-ttu-id="d8e82-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8e82-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



