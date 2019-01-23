---
title: windowsManagementAppHealthState 资源类型
description: Windows 管理应用程序运行状况状态实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 171ae2492eb5077567f4398af678d14044a0b7e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395732"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="d25f9-103">windowsManagementAppHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="d25f9-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="d25f9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d25f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d25f9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d25f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d25f9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d25f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d25f9-107">Windows 管理应用程序运行状况状态实体。</span><span class="sxs-lookup"><span data-stu-id="d25f9-107">Windows management app health state entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d25f9-108">方法</span><span class="sxs-lookup"><span data-stu-id="d25f9-108">Methods</span></span>
|<span data-ttu-id="d25f9-109">方法</span><span class="sxs-lookup"><span data-stu-id="d25f9-109">Method</span></span>|<span data-ttu-id="d25f9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d25f9-110">Return Type</span></span>|<span data-ttu-id="d25f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="d25f9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d25f9-112">列表 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="d25f9-112">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="d25f9-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="d25f9-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="d25f9-114">列出属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d25f9-114">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="d25f9-115">获取 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-115">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="d25f9-116">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-116">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="d25f9-117">读取属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d25f9-117">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="d25f9-118">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-118">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="d25f9-119">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-119">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="d25f9-120">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d25f9-120">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="d25f9-121">删除 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-121">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="d25f9-122">无</span><span class="sxs-lookup"><span data-stu-id="d25f9-122">None</span></span>|<span data-ttu-id="d25f9-123">删除[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="d25f9-123">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="d25f9-124">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-124">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="d25f9-125">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-125">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="d25f9-126">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d25f9-126">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d25f9-127">属性</span><span class="sxs-lookup"><span data-stu-id="d25f9-127">Properties</span></span>
|<span data-ttu-id="d25f9-128">属性</span><span class="sxs-lookup"><span data-stu-id="d25f9-128">Property</span></span>|<span data-ttu-id="d25f9-129">类型</span><span class="sxs-lookup"><span data-stu-id="d25f9-129">Type</span></span>|<span data-ttu-id="d25f9-130">说明</span><span class="sxs-lookup"><span data-stu-id="d25f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d25f9-131">id</span><span class="sxs-lookup"><span data-stu-id="d25f9-131">id</span></span>|<span data-ttu-id="d25f9-132">String</span><span class="sxs-lookup"><span data-stu-id="d25f9-132">String</span></span>|<span data-ttu-id="d25f9-133">Windows 管理应用程序的运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d25f9-133">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="d25f9-134">healthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-134">healthState</span></span>|[<span data-ttu-id="d25f9-135">healthState</span><span class="sxs-lookup"><span data-stu-id="d25f9-135">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="d25f9-136">Windows 管理应用程序的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="d25f9-136">Windows management app health state.</span></span> <span data-ttu-id="d25f9-137">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="d25f9-137">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="d25f9-138">installedVersion</span><span class="sxs-lookup"><span data-stu-id="d25f9-138">installedVersion</span></span>|<span data-ttu-id="d25f9-139">String</span><span class="sxs-lookup"><span data-stu-id="d25f9-139">String</span></span>|<span data-ttu-id="d25f9-140">Windows 管理应用程序安装的版本。</span><span class="sxs-lookup"><span data-stu-id="d25f9-140">Windows management app installed version.</span></span>|
|<span data-ttu-id="d25f9-141">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="d25f9-141">lastCheckInDateTime</span></span>|<span data-ttu-id="d25f9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d25f9-142">DateTimeOffset</span></span>|<span data-ttu-id="d25f9-143">Windows 管理应用程序上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="d25f9-143">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="d25f9-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="d25f9-144">deviceName</span></span>|<span data-ttu-id="d25f9-145">String</span><span class="sxs-lookup"><span data-stu-id="d25f9-145">String</span></span>|<span data-ttu-id="d25f9-146">设备的 Windows 安装管理应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="d25f9-146">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="d25f9-147">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="d25f9-147">deviceOSVersion</span></span>|<span data-ttu-id="d25f9-148">String</span><span class="sxs-lookup"><span data-stu-id="d25f9-148">String</span></span>|<span data-ttu-id="d25f9-149">Windows 10 OS 版本的 Windows 安装管理应用程序的设备。</span><span class="sxs-lookup"><span data-stu-id="d25f9-149">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d25f9-150">关系</span><span class="sxs-lookup"><span data-stu-id="d25f9-150">Relationships</span></span>
<span data-ttu-id="d25f9-151">无</span><span class="sxs-lookup"><span data-stu-id="d25f9-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d25f9-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d25f9-152">JSON Representation</span></span>
<span data-ttu-id="d25f9-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d25f9-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```




