---
title: 更新 windowsManagementAppHealthSummary
description: 更新 windowsManagementAppHealthSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6749c6858f51295b1221afecf802fa088a952a7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965604"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="597a1-103">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="597a1-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="597a1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="597a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="597a1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="597a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="597a1-106">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="597a1-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="597a1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="597a1-107">Prerequisites</span></span>
<span data-ttu-id="597a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="597a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="597a1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="597a1-110">Permission type</span></span>|<span data-ttu-id="597a1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="597a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="597a1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="597a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="597a1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="597a1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="597a1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="597a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="597a1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="597a1-115">Not supported.</span></span>|
|<span data-ttu-id="597a1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="597a1-116">Application</span></span>|<span data-ttu-id="597a1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="597a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="597a1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="597a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="597a1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="597a1-119">Request headers</span></span>
|<span data-ttu-id="597a1-120">标头</span><span class="sxs-lookup"><span data-stu-id="597a1-120">Header</span></span>|<span data-ttu-id="597a1-121">值</span><span class="sxs-lookup"><span data-stu-id="597a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="597a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="597a1-122">Authorization</span></span>|<span data-ttu-id="597a1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="597a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="597a1-124">接受</span><span class="sxs-lookup"><span data-stu-id="597a1-124">Accept</span></span>|<span data-ttu-id="597a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="597a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="597a1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="597a1-126">Request body</span></span>
<span data-ttu-id="597a1-127">在请求正文中, 提供[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="597a1-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="597a1-128">下表显示创建[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="597a1-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="597a1-129">属性</span><span class="sxs-lookup"><span data-stu-id="597a1-129">Property</span></span>|<span data-ttu-id="597a1-130">类型</span><span class="sxs-lookup"><span data-stu-id="597a1-130">Type</span></span>|<span data-ttu-id="597a1-131">说明</span><span class="sxs-lookup"><span data-stu-id="597a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="597a1-132">id</span><span class="sxs-lookup"><span data-stu-id="597a1-132">id</span></span>|<span data-ttu-id="597a1-133">String</span><span class="sxs-lookup"><span data-stu-id="597a1-133">String</span></span>|<span data-ttu-id="597a1-134">Windows management 应用运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="597a1-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="597a1-135">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="597a1-135">healthyDeviceCount</span></span>|<span data-ttu-id="597a1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="597a1-136">Int32</span></span>|<span data-ttu-id="597a1-137">正常的设备计数。</span><span class="sxs-lookup"><span data-stu-id="597a1-137">Healthy device count.</span></span>|
|<span data-ttu-id="597a1-138">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="597a1-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="597a1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="597a1-139">Int32</span></span>|<span data-ttu-id="597a1-140">设备计数不正常。</span><span class="sxs-lookup"><span data-stu-id="597a1-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="597a1-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="597a1-141">unknownDeviceCount</span></span>|<span data-ttu-id="597a1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="597a1-142">Int32</span></span>|<span data-ttu-id="597a1-143">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="597a1-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="597a1-144">响应</span><span class="sxs-lookup"><span data-stu-id="597a1-144">Response</span></span>
<span data-ttu-id="597a1-145">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="597a1-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="597a1-146">示例</span><span class="sxs-lookup"><span data-stu-id="597a1-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="597a1-147">请求</span><span class="sxs-lookup"><span data-stu-id="597a1-147">Request</span></span>
<span data-ttu-id="597a1-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="597a1-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="597a1-149">响应</span><span class="sxs-lookup"><span data-stu-id="597a1-149">Response</span></span>
<span data-ttu-id="597a1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="597a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```




