---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aaca6501f0a1c0fd206583af4e976b9afe9ac2cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869291"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="d3a46-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="d3a46-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="d3a46-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d3a46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3a46-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d3a46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3a46-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d3a46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3a46-107">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3a46-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3a46-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3a46-108">Prerequisites</span></span>
<span data-ttu-id="d3a46-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d3a46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a46-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3a46-111">Permission type</span></span>|<span data-ttu-id="d3a46-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3a46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3a46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a46-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a46-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d3a46-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3a46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3a46-116">Not supported.</span></span>|
|<span data-ttu-id="d3a46-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3a46-117">Application</span></span>|<span data-ttu-id="d3a46-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3a46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a46-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3a46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="d3a46-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3a46-120">Request headers</span></span>
|<span data-ttu-id="d3a46-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3a46-121">Header</span></span>|<span data-ttu-id="d3a46-122">值</span><span class="sxs-lookup"><span data-stu-id="d3a46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3a46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3a46-123">Authorization</span></span>|<span data-ttu-id="d3a46-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3a46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3a46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3a46-125">Accept</span></span>|<span data-ttu-id="d3a46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3a46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a46-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3a46-127">Request body</span></span>
<span data-ttu-id="d3a46-128">在请求正文中，提供[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3a46-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="d3a46-129">下表显示时创建[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d3a46-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="d3a46-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3a46-130">Property</span></span>|<span data-ttu-id="d3a46-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3a46-131">Type</span></span>|<span data-ttu-id="d3a46-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3a46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a46-133">id</span><span class="sxs-lookup"><span data-stu-id="d3a46-133">id</span></span>|<span data-ttu-id="d3a46-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d3a46-134">String</span></span>|<span data-ttu-id="d3a46-135">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d3a46-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="d3a46-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d3a46-136">displayName</span></span>|<span data-ttu-id="d3a46-137">字符串</span><span class="sxs-lookup"><span data-stu-id="d3a46-137">String</span></span>|<span data-ttu-id="d3a46-138">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="d3a46-138">Name of the device management script.</span></span>|
|<span data-ttu-id="d3a46-139">说明</span><span class="sxs-lookup"><span data-stu-id="d3a46-139">description</span></span>|<span data-ttu-id="d3a46-140">字符串</span><span class="sxs-lookup"><span data-stu-id="d3a46-140">String</span></span>|<span data-ttu-id="d3a46-141">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="d3a46-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="d3a46-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d3a46-142">runSchedule</span></span>|[<span data-ttu-id="d3a46-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d3a46-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="d3a46-144">Script to run 时间间隔。</span><span class="sxs-lookup"><span data-stu-id="d3a46-144">The interval for script to run.</span></span> <span data-ttu-id="d3a46-145">如果未定义脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="d3a46-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="d3a46-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="d3a46-146">scriptContent</span></span>|<span data-ttu-id="d3a46-147">Binary</span><span class="sxs-lookup"><span data-stu-id="d3a46-147">Binary</span></span>|<span data-ttu-id="d3a46-148">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="d3a46-148">The script content.</span></span>|
|<span data-ttu-id="d3a46-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3a46-149">createdDateTime</span></span>|<span data-ttu-id="d3a46-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3a46-150">DateTimeOffset</span></span>|<span data-ttu-id="d3a46-151">创建设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3a46-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="d3a46-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3a46-152">lastModifiedDateTime</span></span>|<span data-ttu-id="d3a46-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3a46-153">DateTimeOffset</span></span>|<span data-ttu-id="d3a46-154">日期和设备管理脚本上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="d3a46-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="d3a46-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d3a46-155">runAsAccount</span></span>|[<span data-ttu-id="d3a46-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="d3a46-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d3a46-157">指示执行上下文中运行的设备管理脚本的类型。</span><span class="sxs-lookup"><span data-stu-id="d3a46-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="d3a46-158">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="d3a46-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d3a46-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="d3a46-159">enforceSignatureCheck</span></span>|<span data-ttu-id="d3a46-160">布尔</span><span class="sxs-lookup"><span data-stu-id="d3a46-160">Boolean</span></span>|<span data-ttu-id="d3a46-161">指示是否需要签脚本签名。</span><span class="sxs-lookup"><span data-stu-id="d3a46-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="d3a46-162">fileName</span><span class="sxs-lookup"><span data-stu-id="d3a46-162">fileName</span></span>|<span data-ttu-id="d3a46-163">String</span><span class="sxs-lookup"><span data-stu-id="d3a46-163">String</span></span>|<span data-ttu-id="d3a46-164">脚本文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d3a46-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="d3a46-165">响应</span><span class="sxs-lookup"><span data-stu-id="d3a46-165">Response</span></span>
<span data-ttu-id="d3a46-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3a46-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a46-167">示例</span><span class="sxs-lookup"><span data-stu-id="d3a46-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3a46-168">请求</span><span class="sxs-lookup"><span data-stu-id="d3a46-168">Request</span></span>
<span data-ttu-id="d3a46-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3a46-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 361

{
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```

### <a name="response"></a><span data-ttu-id="d3a46-170">响应</span><span class="sxs-lookup"><span data-stu-id="d3a46-170">Response</span></span>
<span data-ttu-id="d3a46-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3a46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 530

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
  "fileName": "File Name value"
}
```





