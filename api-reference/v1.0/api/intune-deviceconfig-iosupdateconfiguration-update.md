---
title: 更新 iosUpdateConfiguration
description: 更新 iosUpdateConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c3f4743c6586208b773608e48f403f0a23eec2f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756314"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="91f16-103">更新 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="91f16-103">Update iosUpdateConfiguration</span></span>

<span data-ttu-id="91f16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91f16-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91f16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91f16-106">更新 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="91f16-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91f16-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="91f16-107">Prerequisites</span></span>
<span data-ttu-id="91f16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91f16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="91f16-110">Permission type</span></span>|<span data-ttu-id="91f16-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91f16-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91f16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91f16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91f16-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f16-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91f16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91f16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91f16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="91f16-115">Not supported.</span></span>|
|<span data-ttu-id="91f16-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="91f16-116">Application</span></span>|<span data-ttu-id="91f16-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f16-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f16-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91f16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="91f16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="91f16-119">Request headers</span></span>
|<span data-ttu-id="91f16-120">标头</span><span class="sxs-lookup"><span data-stu-id="91f16-120">Header</span></span>|<span data-ttu-id="91f16-121">值</span><span class="sxs-lookup"><span data-stu-id="91f16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91f16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91f16-122">Authorization</span></span>|<span data-ttu-id="91f16-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91f16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91f16-124">接受</span><span class="sxs-lookup"><span data-stu-id="91f16-124">Accept</span></span>|<span data-ttu-id="91f16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91f16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f16-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91f16-126">Request body</span></span>
<span data-ttu-id="91f16-127">在请求正文中，提供 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91f16-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="91f16-128">下表显示创建 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="91f16-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="91f16-129">属性</span><span class="sxs-lookup"><span data-stu-id="91f16-129">Property</span></span>|<span data-ttu-id="91f16-130">类型</span><span class="sxs-lookup"><span data-stu-id="91f16-130">Type</span></span>|<span data-ttu-id="91f16-131">说明</span><span class="sxs-lookup"><span data-stu-id="91f16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f16-132">id</span><span class="sxs-lookup"><span data-stu-id="91f16-132">id</span></span>|<span data-ttu-id="91f16-133">String</span><span class="sxs-lookup"><span data-stu-id="91f16-133">String</span></span>|<span data-ttu-id="91f16-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="91f16-134">Key of the entity.</span></span> <span data-ttu-id="91f16-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f16-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f16-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91f16-136">lastModifiedDateTime</span></span>|<span data-ttu-id="91f16-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f16-137">DateTimeOffset</span></span>|<span data-ttu-id="91f16-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="91f16-138">DateTime the object was last modified.</span></span> <span data-ttu-id="91f16-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f16-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f16-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91f16-140">createdDateTime</span></span>|<span data-ttu-id="91f16-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f16-141">DateTimeOffset</span></span>|<span data-ttu-id="91f16-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="91f16-142">DateTime the object was created.</span></span> <span data-ttu-id="91f16-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f16-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f16-144">说明</span><span class="sxs-lookup"><span data-stu-id="91f16-144">description</span></span>|<span data-ttu-id="91f16-145">String</span><span class="sxs-lookup"><span data-stu-id="91f16-145">String</span></span>|<span data-ttu-id="91f16-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="91f16-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91f16-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f16-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f16-148">displayName</span><span class="sxs-lookup"><span data-stu-id="91f16-148">displayName</span></span>|<span data-ttu-id="91f16-149">String</span><span class="sxs-lookup"><span data-stu-id="91f16-149">String</span></span>|<span data-ttu-id="91f16-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="91f16-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91f16-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f16-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f16-152">version</span><span class="sxs-lookup"><span data-stu-id="91f16-152">version</span></span>|<span data-ttu-id="91f16-153">Int32</span><span class="sxs-lookup"><span data-stu-id="91f16-153">Int32</span></span>|<span data-ttu-id="91f16-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="91f16-154">Version of the device configuration.</span></span> <span data-ttu-id="91f16-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f16-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f16-156">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="91f16-156">activeHoursStart</span></span>|<span data-ttu-id="91f16-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="91f16-157">TimeOfDay</span></span>|<span data-ttu-id="91f16-158">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="91f16-158">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="91f16-159">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="91f16-159">activeHoursEnd</span></span>|<span data-ttu-id="91f16-160">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="91f16-160">TimeOfDay</span></span>|<span data-ttu-id="91f16-161">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="91f16-161">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="91f16-162">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="91f16-162">scheduledInstallDays</span></span>|<span data-ttu-id="91f16-163">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91f16-163">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="91f16-164">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="91f16-164">Days in week for which active hours are configured.</span></span> <span data-ttu-id="91f16-165">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="91f16-165">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="91f16-166">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="91f16-166">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="91f16-167">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="91f16-167">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="91f16-168">Int32</span><span class="sxs-lookup"><span data-stu-id="91f16-168">Int32</span></span>|<span data-ttu-id="91f16-169">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="91f16-169">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="91f16-170">响应</span><span class="sxs-lookup"><span data-stu-id="91f16-170">Response</span></span>
<span data-ttu-id="91f16-171">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91f16-171">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f16-172">示例</span><span class="sxs-lookup"><span data-stu-id="91f16-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="91f16-173">请求</span><span class="sxs-lookup"><span data-stu-id="91f16-173">Request</span></span>
<span data-ttu-id="91f16-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91f16-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91f16-175">响应</span><span class="sxs-lookup"><span data-stu-id="91f16-175">Response</span></span>
<span data-ttu-id="91f16-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91f16-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




