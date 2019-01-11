---
title: windowsManagementAppHealthState 资源类型
description: Windows 管理应用程序运行状况状态实体。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23381aed47ade8f42937f6bc48cfff33b36d1fa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875297"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="47852-103">windowsManagementAppHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="47852-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="47852-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="47852-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47852-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="47852-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47852-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="47852-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47852-107">Windows 管理应用程序运行状况状态实体。</span><span class="sxs-lookup"><span data-stu-id="47852-107">Windows management app health state entity.</span></span>
## <a name="methods"></a><span data-ttu-id="47852-108">方法</span><span class="sxs-lookup"><span data-stu-id="47852-108">Methods</span></span>
|<span data-ttu-id="47852-109">方法</span><span class="sxs-lookup"><span data-stu-id="47852-109">Method</span></span>|<span data-ttu-id="47852-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="47852-110">Return Type</span></span>|<span data-ttu-id="47852-111">说明</span><span class="sxs-lookup"><span data-stu-id="47852-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47852-112">列表 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="47852-112">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="47852-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="47852-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="47852-114">列出属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="47852-114">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="47852-115">获取 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-115">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="47852-116">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-116">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="47852-117">读取属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="47852-117">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="47852-118">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-118">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="47852-119">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-119">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="47852-120">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47852-120">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="47852-121">删除 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-121">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="47852-122">无</span><span class="sxs-lookup"><span data-stu-id="47852-122">None</span></span>|<span data-ttu-id="47852-123">删除[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="47852-123">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="47852-124">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-124">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="47852-125">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="47852-125">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="47852-126">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47852-126">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47852-127">属性</span><span class="sxs-lookup"><span data-stu-id="47852-127">Properties</span></span>
|<span data-ttu-id="47852-128">属性</span><span class="sxs-lookup"><span data-stu-id="47852-128">Property</span></span>|<span data-ttu-id="47852-129">类型</span><span class="sxs-lookup"><span data-stu-id="47852-129">Type</span></span>|<span data-ttu-id="47852-130">说明</span><span class="sxs-lookup"><span data-stu-id="47852-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47852-131">id</span><span class="sxs-lookup"><span data-stu-id="47852-131">id</span></span>|<span data-ttu-id="47852-132">字符串</span><span class="sxs-lookup"><span data-stu-id="47852-132">String</span></span>|<span data-ttu-id="47852-133">Windows 管理应用程序的运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="47852-133">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="47852-134">healthState</span><span class="sxs-lookup"><span data-stu-id="47852-134">healthState</span></span>|[<span data-ttu-id="47852-135">healthState</span><span class="sxs-lookup"><span data-stu-id="47852-135">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="47852-136">Windows 管理应用程序的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="47852-136">Windows management app health state.</span></span> <span data-ttu-id="47852-137">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="47852-137">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="47852-138">installedVersion</span><span class="sxs-lookup"><span data-stu-id="47852-138">installedVersion</span></span>|<span data-ttu-id="47852-139">字符串</span><span class="sxs-lookup"><span data-stu-id="47852-139">String</span></span>|<span data-ttu-id="47852-140">Windows 管理应用程序安装的版本。</span><span class="sxs-lookup"><span data-stu-id="47852-140">Windows management app installed version.</span></span>|
|<span data-ttu-id="47852-141">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="47852-141">lastCheckInDateTime</span></span>|<span data-ttu-id="47852-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47852-142">DateTimeOffset</span></span>|<span data-ttu-id="47852-143">Windows 管理应用程序上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="47852-143">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="47852-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="47852-144">deviceName</span></span>|<span data-ttu-id="47852-145">String</span><span class="sxs-lookup"><span data-stu-id="47852-145">String</span></span>|<span data-ttu-id="47852-146">设备的 Windows 安装管理应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="47852-146">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="47852-147">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="47852-147">deviceOSVersion</span></span>|<span data-ttu-id="47852-148">字符串</span><span class="sxs-lookup"><span data-stu-id="47852-148">String</span></span>|<span data-ttu-id="47852-149">Windows 10 OS 版本的 Windows 安装管理应用程序的设备。</span><span class="sxs-lookup"><span data-stu-id="47852-149">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47852-150">Relationships</span><span class="sxs-lookup"><span data-stu-id="47852-150">Relationships</span></span>
<span data-ttu-id="47852-151">无</span><span class="sxs-lookup"><span data-stu-id="47852-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47852-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47852-152">JSON Representation</span></span>
<span data-ttu-id="47852-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47852-153">Here is a JSON representation of the resource.</span></span>
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





