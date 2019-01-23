---
title: 更新 windowsManagementAppHealthSummary
description: 更新 windowsManagementAppHealthSummary 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7e8c077b8f06b9647e34a18fd5aa92987272e77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394164"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="36703-103">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="36703-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="36703-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="36703-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36703-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36703-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36703-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36703-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36703-107">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="36703-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36703-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="36703-108">Prerequisites</span></span>
<span data-ttu-id="36703-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="36703-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36703-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36703-111">Permission type</span></span>|<span data-ttu-id="36703-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36703-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36703-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36703-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36703-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36703-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36703-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36703-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36703-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36703-116">Not supported.</span></span>|
|<span data-ttu-id="36703-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36703-117">Application</span></span>|<span data-ttu-id="36703-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="36703-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36703-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36703-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="36703-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36703-120">Request headers</span></span>
|<span data-ttu-id="36703-121">标头</span><span class="sxs-lookup"><span data-stu-id="36703-121">Header</span></span>|<span data-ttu-id="36703-122">值</span><span class="sxs-lookup"><span data-stu-id="36703-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36703-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36703-123">Authorization</span></span>|<span data-ttu-id="36703-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36703-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36703-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36703-125">Accept</span></span>|<span data-ttu-id="36703-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36703-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36703-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36703-127">Request body</span></span>
<span data-ttu-id="36703-128">在请求正文中，提供[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36703-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="36703-129">下表显示时创建[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36703-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="36703-130">属性</span><span class="sxs-lookup"><span data-stu-id="36703-130">Property</span></span>|<span data-ttu-id="36703-131">类型</span><span class="sxs-lookup"><span data-stu-id="36703-131">Type</span></span>|<span data-ttu-id="36703-132">说明</span><span class="sxs-lookup"><span data-stu-id="36703-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36703-133">id</span><span class="sxs-lookup"><span data-stu-id="36703-133">id</span></span>|<span data-ttu-id="36703-134">String</span><span class="sxs-lookup"><span data-stu-id="36703-134">String</span></span>|<span data-ttu-id="36703-135">Windows 管理应用程序运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="36703-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="36703-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="36703-136">healthyDeviceCount</span></span>|<span data-ttu-id="36703-137">Int32</span><span class="sxs-lookup"><span data-stu-id="36703-137">Int32</span></span>|<span data-ttu-id="36703-138">正常运行的设备计数。</span><span class="sxs-lookup"><span data-stu-id="36703-138">Healthy device count.</span></span>|
|<span data-ttu-id="36703-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="36703-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="36703-140">Int32</span><span class="sxs-lookup"><span data-stu-id="36703-140">Int32</span></span>|<span data-ttu-id="36703-141">正常设备计数。</span><span class="sxs-lookup"><span data-stu-id="36703-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="36703-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="36703-142">unknownDeviceCount</span></span>|<span data-ttu-id="36703-143">Int32</span><span class="sxs-lookup"><span data-stu-id="36703-143">Int32</span></span>|<span data-ttu-id="36703-144">未知的设备计数。</span><span class="sxs-lookup"><span data-stu-id="36703-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="36703-145">响应</span><span class="sxs-lookup"><span data-stu-id="36703-145">Response</span></span>
<span data-ttu-id="36703-146">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36703-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36703-147">示例</span><span class="sxs-lookup"><span data-stu-id="36703-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="36703-148">请求</span><span class="sxs-lookup"><span data-stu-id="36703-148">Request</span></span>
<span data-ttu-id="36703-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36703-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36703-150">响应</span><span class="sxs-lookup"><span data-stu-id="36703-150">Response</span></span>
<span data-ttu-id="36703-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36703-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




