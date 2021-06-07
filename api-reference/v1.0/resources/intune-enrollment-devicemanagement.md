---
title: deviceManagement 资源类型
description: deviceManagement 资源表示已在 Intune 中预留的租户的集合设备标识，以及可能分配给支持预注册配置的设备标识的注册配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38c93be6c71f97e828901f51c7d6851a346f0bd1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755233"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="928e7-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="928e7-103">deviceManagement resource type</span></span>

<span data-ttu-id="928e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="928e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="928e7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="928e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="928e7-106">deviceManagement 资源表示已在 Intune 中预留的租户的集合设备标识，以及可能分配给支持预注册配置的设备标识的注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="928e7-106">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="928e7-107">方法</span><span class="sxs-lookup"><span data-stu-id="928e7-107">Methods</span></span>
|<span data-ttu-id="928e7-108">方法</span><span class="sxs-lookup"><span data-stu-id="928e7-108">Method</span></span>|<span data-ttu-id="928e7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="928e7-109">Return Type</span></span>|<span data-ttu-id="928e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="928e7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="928e7-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="928e7-111">Get deviceManagement</span></span>](../api/intune-enrollment-devicemanagement-get.md)|[<span data-ttu-id="928e7-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="928e7-112">deviceManagement</span></span>](../resources/intune-enrollment-devicemanagement.md)|<span data-ttu-id="928e7-113">读取 [deviceManagement](../resources/intune-enrollment-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="928e7-113">Read properties and relationships of the [deviceManagement](../resources/intune-enrollment-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="928e7-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="928e7-114">Update deviceManagement</span></span>](../api/intune-enrollment-devicemanagement-update.md)|[<span data-ttu-id="928e7-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="928e7-115">deviceManagement</span></span>](../resources/intune-enrollment-devicemanagement.md)|<span data-ttu-id="928e7-116">更新 [deviceManagement](../resources/intune-enrollment-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="928e7-116">Update the properties of a [deviceManagement](../resources/intune-enrollment-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="928e7-117">属性</span><span class="sxs-lookup"><span data-stu-id="928e7-117">Properties</span></span>
|<span data-ttu-id="928e7-118">属性</span><span class="sxs-lookup"><span data-stu-id="928e7-118">Property</span></span>|<span data-ttu-id="928e7-119">类型</span><span class="sxs-lookup"><span data-stu-id="928e7-119">Type</span></span>|<span data-ttu-id="928e7-120">说明</span><span class="sxs-lookup"><span data-stu-id="928e7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="928e7-121">id</span><span class="sxs-lookup"><span data-stu-id="928e7-121">id</span></span>|<span data-ttu-id="928e7-122">String</span><span class="sxs-lookup"><span data-stu-id="928e7-122">String</span></span>|<span data-ttu-id="928e7-123">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="928e7-123">The GUID for the object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="928e7-124">关系</span><span class="sxs-lookup"><span data-stu-id="928e7-124">Relationships</span></span>
|<span data-ttu-id="928e7-125">关系</span><span class="sxs-lookup"><span data-stu-id="928e7-125">Relationship</span></span>|<span data-ttu-id="928e7-126">类型</span><span class="sxs-lookup"><span data-stu-id="928e7-126">Type</span></span>|<span data-ttu-id="928e7-127">说明</span><span class="sxs-lookup"><span data-stu-id="928e7-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="928e7-128">windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="928e7-128">windowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="928e7-129">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="928e7-129">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="928e7-130">该Windows autopilot 设备标识包含集合。</span><span class="sxs-lookup"><span data-stu-id="928e7-130">The Windows autopilot device identities contained collection.</span></span>|
|<span data-ttu-id="928e7-131">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="928e7-131">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="928e7-132">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="928e7-132">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="928e7-133">导入的 Windows AutoPilot 设备的集合。</span><span class="sxs-lookup"><span data-stu-id="928e7-133">Collection of imported Windows autopilot devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="928e7-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="928e7-134">JSON Representation</span></span>
<span data-ttu-id="928e7-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="928e7-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




