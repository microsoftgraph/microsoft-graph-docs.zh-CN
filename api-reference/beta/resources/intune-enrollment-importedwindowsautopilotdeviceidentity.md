---
title: importedWindowsAutopilotDeviceIdentity 资源类型
description: 导入 Windows AutoPilot 的设备。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6b64b03e9fcc80a72a027317e29b564f127470a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408220"
---
# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a><span data-ttu-id="0c08c-103">importedWindowsAutopilotDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c08c-103">importedWindowsAutopilotDeviceIdentity resource type</span></span>

> <span data-ttu-id="0c08c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0c08c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c08c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c08c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c08c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c08c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c08c-107">导入 Windows AutoPilot 的设备。</span><span class="sxs-lookup"><span data-stu-id="0c08c-107">Imported windows autopilot devices.</span></span>

## <a name="methods"></a><span data-ttu-id="0c08c-108">方法</span><span class="sxs-lookup"><span data-stu-id="0c08c-108">Methods</span></span>
|<span data-ttu-id="0c08c-109">方法</span><span class="sxs-lookup"><span data-stu-id="0c08c-109">Method</span></span>|<span data-ttu-id="0c08c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c08c-110">Return Type</span></span>|<span data-ttu-id="0c08c-111">说明</span><span class="sxs-lookup"><span data-stu-id="0c08c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c08c-112">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="0c08c-112">List importedWindowsAutopilotDeviceIdentities</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-list.md)|<span data-ttu-id="0c08c-113">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c08c-113">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="0c08c-114">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="0c08c-114">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="0c08c-115">获取 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-115">Get importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-get.md)|[<span data-ttu-id="0c08c-116">importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-116">importedWindowsAutopilotDeviceIdentity</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|<span data-ttu-id="0c08c-117">阅读属性和关系[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0c08c-117">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="0c08c-118">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-118">Create importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-create.md)|[<span data-ttu-id="0c08c-119">importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-119">importedWindowsAutopilotDeviceIdentity</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|<span data-ttu-id="0c08c-120">创建新[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0c08c-120">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="0c08c-121">删除 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-121">Delete importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-delete.md)|<span data-ttu-id="0c08c-122">无</span><span class="sxs-lookup"><span data-stu-id="0c08c-122">None</span></span>|<span data-ttu-id="0c08c-123">删除[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="0c08c-123">Deletes a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>|
|[<span data-ttu-id="0c08c-124">更新 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-124">Update importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-update.md)|[<span data-ttu-id="0c08c-125">importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0c08c-125">importedWindowsAutopilotDeviceIdentity</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|<span data-ttu-id="0c08c-126">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0c08c-126">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c08c-127">属性</span><span class="sxs-lookup"><span data-stu-id="0c08c-127">Properties</span></span>
|<span data-ttu-id="0c08c-128">属性</span><span class="sxs-lookup"><span data-stu-id="0c08c-128">Property</span></span>|<span data-ttu-id="0c08c-129">类型</span><span class="sxs-lookup"><span data-stu-id="0c08c-129">Type</span></span>|<span data-ttu-id="0c08c-130">说明</span><span class="sxs-lookup"><span data-stu-id="0c08c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c08c-131">id</span><span class="sxs-lookup"><span data-stu-id="0c08c-131">id</span></span>|<span data-ttu-id="0c08c-132">String</span><span class="sxs-lookup"><span data-stu-id="0c08c-132">String</span></span>|<span data-ttu-id="0c08c-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="0c08c-133">The GUID for the object</span></span>|
|<span data-ttu-id="0c08c-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c08c-134">orderIdentifier</span></span>|<span data-ttu-id="0c08c-135">String</span><span class="sxs-lookup"><span data-stu-id="0c08c-135">String</span></span>|<span data-ttu-id="0c08c-136">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="0c08c-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0c08c-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0c08c-137">serialNumber</span></span>|<span data-ttu-id="0c08c-138">String</span><span class="sxs-lookup"><span data-stu-id="0c08c-138">String</span></span>|<span data-ttu-id="0c08c-139">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="0c08c-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0c08c-140">productKey</span><span class="sxs-lookup"><span data-stu-id="0c08c-140">productKey</span></span>|<span data-ttu-id="0c08c-141">String</span><span class="sxs-lookup"><span data-stu-id="0c08c-141">String</span></span>|<span data-ttu-id="0c08c-142">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="0c08c-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0c08c-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c08c-143">hardwareIdentifier</span></span>|<span data-ttu-id="0c08c-144">Binary</span><span class="sxs-lookup"><span data-stu-id="0c08c-144">Binary</span></span>|<span data-ttu-id="0c08c-145">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="0c08c-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0c08c-146">state</span><span class="sxs-lookup"><span data-stu-id="0c08c-146">state</span></span>|[<span data-ttu-id="0c08c-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="0c08c-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="0c08c-148">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0c08c-148">Current state of the imported device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c08c-149">关系</span><span class="sxs-lookup"><span data-stu-id="0c08c-149">Relationships</span></span>
<span data-ttu-id="0c08c-150">无</span><span class="sxs-lookup"><span data-stu-id="0c08c-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c08c-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c08c-151">JSON Representation</span></span>
<span data-ttu-id="0c08c-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c08c-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "String",
    "deviceRegistrationId": "String",
    "deviceErrorCode": 1024,
    "deviceErrorName": "String"
  }
}
```




