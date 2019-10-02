---
title: 创建 iosUpdateConfiguration
description: 创建新的 iosUpdateConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1092952c2286f8a52096fb63068a66710a29d942
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366270"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="88d09-103">创建 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="88d09-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="88d09-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88d09-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88d09-105">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88d09-105">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88d09-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="88d09-106">Prerequisites</span></span>
<span data-ttu-id="88d09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88d09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88d09-109">Permission type</span></span>|<span data-ttu-id="88d09-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88d09-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88d09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88d09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88d09-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88d09-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88d09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88d09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88d09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88d09-114">Not supported.</span></span>|
|<span data-ttu-id="88d09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88d09-115">Application</span></span>|<span data-ttu-id="88d09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88d09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88d09-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88d09-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="88d09-118">请求头</span><span class="sxs-lookup"><span data-stu-id="88d09-118">Request headers</span></span>
|<span data-ttu-id="88d09-119">标头</span><span class="sxs-lookup"><span data-stu-id="88d09-119">Header</span></span>|<span data-ttu-id="88d09-120">值</span><span class="sxs-lookup"><span data-stu-id="88d09-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88d09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88d09-121">Authorization</span></span>|<span data-ttu-id="88d09-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88d09-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88d09-123">接受</span><span class="sxs-lookup"><span data-stu-id="88d09-123">Accept</span></span>|<span data-ttu-id="88d09-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88d09-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88d09-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="88d09-125">Request body</span></span>
<span data-ttu-id="88d09-126">在请求正文中，提供 iosUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88d09-126">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="88d09-127">下表显示创建 iosUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88d09-127">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="88d09-128">属性</span><span class="sxs-lookup"><span data-stu-id="88d09-128">Property</span></span>|<span data-ttu-id="88d09-129">类型</span><span class="sxs-lookup"><span data-stu-id="88d09-129">Type</span></span>|<span data-ttu-id="88d09-130">说明</span><span class="sxs-lookup"><span data-stu-id="88d09-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d09-131">id</span><span class="sxs-lookup"><span data-stu-id="88d09-131">id</span></span>|<span data-ttu-id="88d09-132">字符串</span><span class="sxs-lookup"><span data-stu-id="88d09-132">String</span></span>|<span data-ttu-id="88d09-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88d09-133">Key of the entity.</span></span> <span data-ttu-id="88d09-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d09-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d09-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88d09-135">lastModifiedDateTime</span></span>|<span data-ttu-id="88d09-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88d09-136">DateTimeOffset</span></span>|<span data-ttu-id="88d09-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88d09-137">DateTime the object was last modified.</span></span> <span data-ttu-id="88d09-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d09-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d09-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88d09-139">createdDateTime</span></span>|<span data-ttu-id="88d09-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88d09-140">DateTimeOffset</span></span>|<span data-ttu-id="88d09-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88d09-141">DateTime the object was created.</span></span> <span data-ttu-id="88d09-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d09-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d09-143">说明</span><span class="sxs-lookup"><span data-stu-id="88d09-143">description</span></span>|<span data-ttu-id="88d09-144">String</span><span class="sxs-lookup"><span data-stu-id="88d09-144">String</span></span>|<span data-ttu-id="88d09-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="88d09-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88d09-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d09-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d09-147">displayName</span><span class="sxs-lookup"><span data-stu-id="88d09-147">displayName</span></span>|<span data-ttu-id="88d09-148">String</span><span class="sxs-lookup"><span data-stu-id="88d09-148">String</span></span>|<span data-ttu-id="88d09-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="88d09-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88d09-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d09-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d09-151">version</span><span class="sxs-lookup"><span data-stu-id="88d09-151">version</span></span>|<span data-ttu-id="88d09-152">Int32</span><span class="sxs-lookup"><span data-stu-id="88d09-152">Int32</span></span>|<span data-ttu-id="88d09-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="88d09-153">Version of the device configuration.</span></span> <span data-ttu-id="88d09-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88d09-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88d09-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="88d09-155">activeHoursStart</span></span>|<span data-ttu-id="88d09-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="88d09-156">TimeOfDay</span></span>|<span data-ttu-id="88d09-157">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="88d09-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="88d09-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="88d09-158">activeHoursEnd</span></span>|<span data-ttu-id="88d09-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="88d09-159">TimeOfDay</span></span>|<span data-ttu-id="88d09-160">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="88d09-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="88d09-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="88d09-161">scheduledInstallDays</span></span>|<span data-ttu-id="88d09-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="88d09-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="88d09-163">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="88d09-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="88d09-164">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="88d09-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="88d09-165">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="88d09-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="88d09-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="88d09-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="88d09-167">Int32</span><span class="sxs-lookup"><span data-stu-id="88d09-167">Int32</span></span>|<span data-ttu-id="88d09-168">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="88d09-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="88d09-169">响应</span><span class="sxs-lookup"><span data-stu-id="88d09-169">Response</span></span>
<span data-ttu-id="88d09-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88d09-170">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88d09-171">示例</span><span class="sxs-lookup"><span data-stu-id="88d09-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="88d09-172">请求</span><span class="sxs-lookup"><span data-stu-id="88d09-172">Request</span></span>
<span data-ttu-id="88d09-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88d09-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="88d09-174">响应</span><span class="sxs-lookup"><span data-stu-id="88d09-174">Response</span></span>
<span data-ttu-id="88d09-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88d09-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




