---
title: 更新 deviceManagementScriptRunSummary
description: 更新 deviceManagementScriptRunSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d2a0ba2a7dfbd44cd5e756010239caee285fe090
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954699"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="3ec26-103">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="3ec26-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="3ec26-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3ec26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ec26-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ec26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ec26-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3ec26-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ec26-107">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3ec26-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ec26-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ec26-108">Prerequisites</span></span>
<span data-ttu-id="3ec26-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3ec26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec26-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ec26-111">Permission type</span></span>|<span data-ttu-id="3ec26-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3ec26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ec26-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ec26-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec26-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3ec26-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ec26-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec26-116">Not supported.</span></span>|
|<span data-ttu-id="3ec26-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec26-117">Application</span></span>|<span data-ttu-id="3ec26-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec26-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ec26-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ec26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="3ec26-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec26-120">Request headers</span></span>
|<span data-ttu-id="3ec26-121">标头</span><span class="sxs-lookup"><span data-stu-id="3ec26-121">Header</span></span>|<span data-ttu-id="3ec26-122">值</span><span class="sxs-lookup"><span data-stu-id="3ec26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ec26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec26-123">Authorization</span></span>|<span data-ttu-id="3ec26-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ec26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ec26-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ec26-125">Accept</span></span>|<span data-ttu-id="3ec26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ec26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec26-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec26-127">Request body</span></span>
<span data-ttu-id="3ec26-128">在请求正文中，提供[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ec26-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="3ec26-129">下表显示时创建[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3ec26-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="3ec26-130">属性</span><span class="sxs-lookup"><span data-stu-id="3ec26-130">Property</span></span>|<span data-ttu-id="3ec26-131">类型</span><span class="sxs-lookup"><span data-stu-id="3ec26-131">Type</span></span>|<span data-ttu-id="3ec26-132">说明</span><span class="sxs-lookup"><span data-stu-id="3ec26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ec26-133">id</span><span class="sxs-lookup"><span data-stu-id="3ec26-133">id</span></span>|<span data-ttu-id="3ec26-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3ec26-134">String</span></span>|<span data-ttu-id="3ec26-135">运行摘要实体的设备管理脚本的键。</span><span class="sxs-lookup"><span data-stu-id="3ec26-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="3ec26-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ec26-136">successDeviceCount</span></span>|<span data-ttu-id="3ec26-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec26-137">Int32</span></span>|<span data-ttu-id="3ec26-138">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="3ec26-138">Success device count.</span></span>|
|<span data-ttu-id="3ec26-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ec26-139">errorDeviceCount</span></span>|<span data-ttu-id="3ec26-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec26-140">Int32</span></span>|<span data-ttu-id="3ec26-141">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="3ec26-141">Error device count.</span></span>|
|<span data-ttu-id="3ec26-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="3ec26-142">successUserCount</span></span>|<span data-ttu-id="3ec26-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec26-143">Int32</span></span>|<span data-ttu-id="3ec26-144">成功用户计数。</span><span class="sxs-lookup"><span data-stu-id="3ec26-144">Success user count.</span></span>|
|<span data-ttu-id="3ec26-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="3ec26-145">errorUserCount</span></span>|<span data-ttu-id="3ec26-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec26-146">Int32</span></span>|<span data-ttu-id="3ec26-147">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="3ec26-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="3ec26-148">响应</span><span class="sxs-lookup"><span data-stu-id="3ec26-148">Response</span></span>
<span data-ttu-id="3ec26-149">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3ec26-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec26-150">示例</span><span class="sxs-lookup"><span data-stu-id="3ec26-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ec26-151">请求</span><span class="sxs-lookup"><span data-stu-id="3ec26-151">Request</span></span>
<span data-ttu-id="3ec26-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec26-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 108

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="3ec26-153">响应</span><span class="sxs-lookup"><span data-stu-id="3ec26-153">Response</span></span>
<span data-ttu-id="3ec26-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ec26-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





