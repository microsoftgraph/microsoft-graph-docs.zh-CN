---
title: 创建 iosUpdateConfiguration
description: 创建新的 iosUpdateConfiguration 对象。
ms.openlocfilehash: 65acd8334cc53e637563cae45d4a6d5721405843
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010783"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="db36a-103">创建 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="db36a-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="db36a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="db36a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db36a-105">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db36a-105">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db36a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="db36a-106">Prerequisites</span></span>
<span data-ttu-id="db36a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="db36a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db36a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db36a-109">Permission type</span></span>|<span data-ttu-id="db36a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db36a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db36a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db36a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="db36a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db36a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db36a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db36a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db36a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db36a-114">Not supported.</span></span>|
|<span data-ttu-id="db36a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db36a-115">Application</span></span>|<span data-ttu-id="db36a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db36a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db36a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db36a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db36a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db36a-118">Request headers</span></span>
|<span data-ttu-id="db36a-119">标头</span><span class="sxs-lookup"><span data-stu-id="db36a-119">Header</span></span>|<span data-ttu-id="db36a-120">值</span><span class="sxs-lookup"><span data-stu-id="db36a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db36a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db36a-121">Authorization</span></span>|<span data-ttu-id="db36a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db36a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db36a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="db36a-123">Accept</span></span>|<span data-ttu-id="db36a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="db36a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db36a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="db36a-125">Request body</span></span>
<span data-ttu-id="db36a-126">在请求正文中，提供 iosUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db36a-126">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="db36a-127">下表显示创建 iosUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db36a-127">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="db36a-128">属性</span><span class="sxs-lookup"><span data-stu-id="db36a-128">Property</span></span>|<span data-ttu-id="db36a-129">类型</span><span class="sxs-lookup"><span data-stu-id="db36a-129">Type</span></span>|<span data-ttu-id="db36a-130">说明</span><span class="sxs-lookup"><span data-stu-id="db36a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db36a-131">id</span><span class="sxs-lookup"><span data-stu-id="db36a-131">id</span></span>|<span data-ttu-id="db36a-132">String</span><span class="sxs-lookup"><span data-stu-id="db36a-132">String</span></span>|<span data-ttu-id="db36a-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db36a-133">Key of the entity.</span></span> <span data-ttu-id="db36a-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db36a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db36a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="db36a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db36a-136">DateTimeOffset</span></span>|<span data-ttu-id="db36a-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="db36a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="db36a-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db36a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db36a-139">createdDateTime</span></span>|<span data-ttu-id="db36a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db36a-140">DateTimeOffset</span></span>|<span data-ttu-id="db36a-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="db36a-141">DateTime the object was created.</span></span> <span data-ttu-id="db36a-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db36a-143">description</span><span class="sxs-lookup"><span data-stu-id="db36a-143">description</span></span>|<span data-ttu-id="db36a-144">String</span><span class="sxs-lookup"><span data-stu-id="db36a-144">String</span></span>|<span data-ttu-id="db36a-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="db36a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db36a-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db36a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="db36a-147">displayName</span></span>|<span data-ttu-id="db36a-148">String</span><span class="sxs-lookup"><span data-stu-id="db36a-148">String</span></span>|<span data-ttu-id="db36a-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="db36a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db36a-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db36a-151">version</span><span class="sxs-lookup"><span data-stu-id="db36a-151">version</span></span>|<span data-ttu-id="db36a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="db36a-152">Int32</span></span>|<span data-ttu-id="db36a-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="db36a-153">Version of the device configuration.</span></span> <span data-ttu-id="db36a-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db36a-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="db36a-155">activeHoursStart</span></span>|<span data-ttu-id="db36a-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="db36a-156">TimeOfDay</span></span>|<span data-ttu-id="db36a-157">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="db36a-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="db36a-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="db36a-158">activeHoursEnd</span></span>|<span data-ttu-id="db36a-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="db36a-159">TimeOfDay</span></span>|<span data-ttu-id="db36a-160">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="db36a-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="db36a-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="db36a-161">scheduledInstallDays</span></span>|<span data-ttu-id="db36a-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="db36a-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="db36a-163">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="db36a-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="db36a-164">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="db36a-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="db36a-165">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="db36a-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="db36a-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="db36a-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="db36a-167">Int32</span><span class="sxs-lookup"><span data-stu-id="db36a-167">Int32</span></span>|<span data-ttu-id="db36a-168">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="db36a-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="db36a-169">响应</span><span class="sxs-lookup"><span data-stu-id="db36a-169">Response</span></span>
<span data-ttu-id="db36a-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db36a-170">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db36a-171">示例</span><span class="sxs-lookup"><span data-stu-id="db36a-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="db36a-172">请求</span><span class="sxs-lookup"><span data-stu-id="db36a-172">Request</span></span>
<span data-ttu-id="db36a-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db36a-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db36a-174">响应</span><span class="sxs-lookup"><span data-stu-id="db36a-174">Response</span></span>
<span data-ttu-id="db36a-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db36a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



