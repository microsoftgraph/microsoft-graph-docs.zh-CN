---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7cdf0364745f97beec777b6971ab096e43e916ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399008"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="883e3-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="883e3-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="883e3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="883e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="883e3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="883e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="883e3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="883e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="883e3-107">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="883e3-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="883e3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="883e3-108">Prerequisites</span></span>
<span data-ttu-id="883e3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="883e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="883e3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="883e3-111">Permission type</span></span>|<span data-ttu-id="883e3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="883e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="883e3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="883e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="883e3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="883e3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="883e3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="883e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="883e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="883e3-116">Not supported.</span></span>|
|<span data-ttu-id="883e3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="883e3-117">Application</span></span>|<span data-ttu-id="883e3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="883e3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="883e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="883e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="883e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="883e3-120">Request headers</span></span>
|<span data-ttu-id="883e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="883e3-121">Header</span></span>|<span data-ttu-id="883e3-122">值</span><span class="sxs-lookup"><span data-stu-id="883e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="883e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="883e3-123">Authorization</span></span>|<span data-ttu-id="883e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="883e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="883e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="883e3-125">Accept</span></span>|<span data-ttu-id="883e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="883e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="883e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="883e3-127">Request body</span></span>
<span data-ttu-id="883e3-128">在请求正文中，提供[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="883e3-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="883e3-129">下表显示时创建[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="883e3-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="883e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="883e3-130">Property</span></span>|<span data-ttu-id="883e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="883e3-131">Type</span></span>|<span data-ttu-id="883e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="883e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="883e3-133">id</span><span class="sxs-lookup"><span data-stu-id="883e3-133">id</span></span>|<span data-ttu-id="883e3-134">String</span><span class="sxs-lookup"><span data-stu-id="883e3-134">String</span></span>|<span data-ttu-id="883e3-135">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="883e3-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="883e3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="883e3-136">displayName</span></span>|<span data-ttu-id="883e3-137">String</span><span class="sxs-lookup"><span data-stu-id="883e3-137">String</span></span>|<span data-ttu-id="883e3-138">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="883e3-138">Name of the device management script.</span></span>|
|<span data-ttu-id="883e3-139">说明</span><span class="sxs-lookup"><span data-stu-id="883e3-139">description</span></span>|<span data-ttu-id="883e3-140">String</span><span class="sxs-lookup"><span data-stu-id="883e3-140">String</span></span>|<span data-ttu-id="883e3-141">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="883e3-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="883e3-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="883e3-142">runSchedule</span></span>|[<span data-ttu-id="883e3-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="883e3-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="883e3-144">Script to run 时间间隔。</span><span class="sxs-lookup"><span data-stu-id="883e3-144">The interval for script to run.</span></span> <span data-ttu-id="883e3-145">如果未定义脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="883e3-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="883e3-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="883e3-146">scriptContent</span></span>|<span data-ttu-id="883e3-147">Binary</span><span class="sxs-lookup"><span data-stu-id="883e3-147">Binary</span></span>|<span data-ttu-id="883e3-148">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="883e3-148">The script content.</span></span>|
|<span data-ttu-id="883e3-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="883e3-149">createdDateTime</span></span>|<span data-ttu-id="883e3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="883e3-150">DateTimeOffset</span></span>|<span data-ttu-id="883e3-151">创建设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="883e3-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="883e3-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="883e3-152">lastModifiedDateTime</span></span>|<span data-ttu-id="883e3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="883e3-153">DateTimeOffset</span></span>|<span data-ttu-id="883e3-154">日期和设备管理脚本上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="883e3-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="883e3-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="883e3-155">runAsAccount</span></span>|[<span data-ttu-id="883e3-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="883e3-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="883e3-157">指示执行上下文中运行的设备管理脚本的类型。</span><span class="sxs-lookup"><span data-stu-id="883e3-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="883e3-158">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="883e3-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="883e3-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="883e3-159">enforceSignatureCheck</span></span>|<span data-ttu-id="883e3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="883e3-160">Boolean</span></span>|<span data-ttu-id="883e3-161">指示是否需要签脚本签名。</span><span class="sxs-lookup"><span data-stu-id="883e3-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="883e3-162">fileName</span><span class="sxs-lookup"><span data-stu-id="883e3-162">fileName</span></span>|<span data-ttu-id="883e3-163">String</span><span class="sxs-lookup"><span data-stu-id="883e3-163">String</span></span>|<span data-ttu-id="883e3-164">脚本文件的名称。</span><span class="sxs-lookup"><span data-stu-id="883e3-164">Script file name.</span></span>|
|<span data-ttu-id="883e3-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="883e3-165">roleScopeTagIds</span></span>|<span data-ttu-id="883e3-166">String 集合</span><span class="sxs-lookup"><span data-stu-id="883e3-166">String collection</span></span>|<span data-ttu-id="883e3-167">此 PowerShellScript 实例范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="883e3-167">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="883e3-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="883e3-168">runAs32Bit</span></span>|<span data-ttu-id="883e3-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="883e3-169">Boolean</span></span>|<span data-ttu-id="883e3-170">一个值，该值的 PowerShell 脚本是否应运行 32 位</span><span class="sxs-lookup"><span data-stu-id="883e3-170">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="883e3-171">响应</span><span class="sxs-lookup"><span data-stu-id="883e3-171">Response</span></span>
<span data-ttu-id="883e3-172">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="883e3-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="883e3-173">示例</span><span class="sxs-lookup"><span data-stu-id="883e3-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="883e3-174">请求</span><span class="sxs-lookup"><span data-stu-id="883e3-174">Request</span></span>
<span data-ttu-id="883e3-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="883e3-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="883e3-176">响应</span><span class="sxs-lookup"><span data-stu-id="883e3-176">Response</span></span>
<span data-ttu-id="883e3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="883e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```




