---
title: importedWindowsAutopilotDeviceIdentity 资源类型
description: 导入 Windows AutoPilot 的设备。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14d37dcd8f976a5d2bfadcac452750093a3a5d97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929785"
---
# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a><span data-ttu-id="eacf2-103">importedWindowsAutopilotDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="eacf2-103">importedWindowsAutopilotDeviceIdentity resource type</span></span>

> <span data-ttu-id="eacf2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eacf2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eacf2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eacf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eacf2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eacf2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eacf2-107">导入 Windows AutoPilot 的设备。</span><span class="sxs-lookup"><span data-stu-id="eacf2-107">Imported windows autopilot devices.</span></span>
## <a name="methods"></a><span data-ttu-id="eacf2-108">方法</span><span class="sxs-lookup"><span data-stu-id="eacf2-108">Methods</span></span>
|<span data-ttu-id="eacf2-109">方法</span><span class="sxs-lookup"><span data-stu-id="eacf2-109">Method</span></span>|<span data-ttu-id="eacf2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="eacf2-110">Return Type</span></span>|<span data-ttu-id="eacf2-111">说明</span><span class="sxs-lookup"><span data-stu-id="eacf2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eacf2-112">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="eacf2-112">List importedWindowsAutopilotDeviceIdentities</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-list.md)|<span data-ttu-id="eacf2-113">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eacf2-113">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="eacf2-114">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="eacf2-114">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="eacf2-115">获取 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-115">Get importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-get.md)|[<span data-ttu-id="eacf2-116">importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-116">importedWindowsAutopilotDeviceIdentity</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|<span data-ttu-id="eacf2-117">阅读属性和关系[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eacf2-117">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="eacf2-118">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-118">Create importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-create.md)|[<span data-ttu-id="eacf2-119">importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-119">importedWindowsAutopilotDeviceIdentity</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|<span data-ttu-id="eacf2-120">创建新[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eacf2-120">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="eacf2-121">删除 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-121">Delete importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-delete.md)|<span data-ttu-id="eacf2-122">无</span><span class="sxs-lookup"><span data-stu-id="eacf2-122">None</span></span>|<span data-ttu-id="eacf2-123">删除[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="eacf2-123">Deletes a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>|
|[<span data-ttu-id="eacf2-124">更新 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-124">Update importedWindowsAutopilotDeviceIdentity</span></span>](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-update.md)|[<span data-ttu-id="eacf2-125">importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eacf2-125">importedWindowsAutopilotDeviceIdentity</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|<span data-ttu-id="eacf2-126">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eacf2-126">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eacf2-127">属性</span><span class="sxs-lookup"><span data-stu-id="eacf2-127">Properties</span></span>
|<span data-ttu-id="eacf2-128">属性</span><span class="sxs-lookup"><span data-stu-id="eacf2-128">Property</span></span>|<span data-ttu-id="eacf2-129">类型</span><span class="sxs-lookup"><span data-stu-id="eacf2-129">Type</span></span>|<span data-ttu-id="eacf2-130">说明</span><span class="sxs-lookup"><span data-stu-id="eacf2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eacf2-131">id</span><span class="sxs-lookup"><span data-stu-id="eacf2-131">id</span></span>|<span data-ttu-id="eacf2-132">字符串</span><span class="sxs-lookup"><span data-stu-id="eacf2-132">String</span></span>|<span data-ttu-id="eacf2-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="eacf2-133">The GUID for the object</span></span>|
|<span data-ttu-id="eacf2-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="eacf2-134">orderIdentifier</span></span>|<span data-ttu-id="eacf2-135">字符串</span><span class="sxs-lookup"><span data-stu-id="eacf2-135">String</span></span>|<span data-ttu-id="eacf2-136">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="eacf2-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eacf2-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="eacf2-137">serialNumber</span></span>|<span data-ttu-id="eacf2-138">字符串</span><span class="sxs-lookup"><span data-stu-id="eacf2-138">String</span></span>|<span data-ttu-id="eacf2-139">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="eacf2-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eacf2-140">productKey</span><span class="sxs-lookup"><span data-stu-id="eacf2-140">productKey</span></span>|<span data-ttu-id="eacf2-141">字符串</span><span class="sxs-lookup"><span data-stu-id="eacf2-141">String</span></span>|<span data-ttu-id="eacf2-142">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="eacf2-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eacf2-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="eacf2-143">hardwareIdentifier</span></span>|<span data-ttu-id="eacf2-144">Binary</span><span class="sxs-lookup"><span data-stu-id="eacf2-144">Binary</span></span>|<span data-ttu-id="eacf2-145">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="eacf2-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eacf2-146">状态</span><span class="sxs-lookup"><span data-stu-id="eacf2-146">state</span></span>|[<span data-ttu-id="eacf2-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="eacf2-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="eacf2-148">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="eacf2-148">Current state of the imported device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eacf2-149">关系</span><span class="sxs-lookup"><span data-stu-id="eacf2-149">Relationships</span></span>
<span data-ttu-id="eacf2-150">无</span><span class="sxs-lookup"><span data-stu-id="eacf2-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eacf2-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eacf2-151">JSON Representation</span></span>
<span data-ttu-id="eacf2-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eacf2-152">Here is a JSON representation of the resource.</span></span>
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





