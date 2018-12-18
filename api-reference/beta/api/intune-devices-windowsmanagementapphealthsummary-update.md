---
title: 更新 windowsManagementAppHealthSummary
description: 更新 windowsManagementAppHealthSummary 对象的属性。
author: tfitzmac
ms.openlocfilehash: 274ffcc65706f7d730815d4a8350af2dee68f763
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307068"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="10195-103">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="10195-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="10195-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="10195-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10195-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="10195-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10195-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10195-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10195-107">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10195-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10195-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="10195-108">Prerequisites</span></span>
<span data-ttu-id="10195-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="10195-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10195-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10195-111">Permission type</span></span>|<span data-ttu-id="10195-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10195-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10195-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10195-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10195-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10195-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="10195-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10195-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10195-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10195-116">Not supported.</span></span>|
|<span data-ttu-id="10195-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="10195-117">Application</span></span>|<span data-ttu-id="10195-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="10195-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10195-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10195-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="10195-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="10195-120">Request headers</span></span>
|<span data-ttu-id="10195-121">标头</span><span class="sxs-lookup"><span data-stu-id="10195-121">Header</span></span>|<span data-ttu-id="10195-122">值</span><span class="sxs-lookup"><span data-stu-id="10195-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10195-123">授权</span><span class="sxs-lookup"><span data-stu-id="10195-123">Authorization</span></span>|<span data-ttu-id="10195-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10195-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10195-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10195-125">Accept</span></span>|<span data-ttu-id="10195-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10195-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10195-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10195-127">Request body</span></span>
<span data-ttu-id="10195-128">在请求正文中，提供[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10195-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="10195-129">下表显示时创建[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="10195-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="10195-130">属性</span><span class="sxs-lookup"><span data-stu-id="10195-130">Property</span></span>|<span data-ttu-id="10195-131">类型</span><span class="sxs-lookup"><span data-stu-id="10195-131">Type</span></span>|<span data-ttu-id="10195-132">说明</span><span class="sxs-lookup"><span data-stu-id="10195-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10195-133">id</span><span class="sxs-lookup"><span data-stu-id="10195-133">id</span></span>|<span data-ttu-id="10195-134">字符串</span><span class="sxs-lookup"><span data-stu-id="10195-134">String</span></span>|<span data-ttu-id="10195-135">Windows 管理应用程序运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="10195-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="10195-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10195-136">healthyDeviceCount</span></span>|<span data-ttu-id="10195-137">Int32</span><span class="sxs-lookup"><span data-stu-id="10195-137">Int32</span></span>|<span data-ttu-id="10195-138">正常运行的设备计数。</span><span class="sxs-lookup"><span data-stu-id="10195-138">Healthy device count.</span></span>|
|<span data-ttu-id="10195-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10195-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="10195-140">Int32</span><span class="sxs-lookup"><span data-stu-id="10195-140">Int32</span></span>|<span data-ttu-id="10195-141">正常设备计数。</span><span class="sxs-lookup"><span data-stu-id="10195-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="10195-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10195-142">unknownDeviceCount</span></span>|<span data-ttu-id="10195-143">Int32</span><span class="sxs-lookup"><span data-stu-id="10195-143">Int32</span></span>|<span data-ttu-id="10195-144">未知的设备计数。</span><span class="sxs-lookup"><span data-stu-id="10195-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="10195-145">响应</span><span class="sxs-lookup"><span data-stu-id="10195-145">Response</span></span>
<span data-ttu-id="10195-146">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10195-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10195-147">示例</span><span class="sxs-lookup"><span data-stu-id="10195-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="10195-148">请求</span><span class="sxs-lookup"><span data-stu-id="10195-148">Request</span></span>
<span data-ttu-id="10195-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10195-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 89

{
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="10195-150">响应</span><span class="sxs-lookup"><span data-stu-id="10195-150">Response</span></span>
<span data-ttu-id="10195-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10195-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





