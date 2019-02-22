---
title: windowsManagementAppHealthState 资源类型
description: Windows management 应用运行状况状态实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8841b79b9a284a15999db701e82a2b5062e2930b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148536"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="c8143-103">windowsManagementAppHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8143-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="c8143-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8143-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8143-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8143-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8143-106">Windows management 应用运行状况状态实体。</span><span class="sxs-lookup"><span data-stu-id="c8143-106">Windows management app health state entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c8143-107">方法</span><span class="sxs-lookup"><span data-stu-id="c8143-107">Methods</span></span>
|<span data-ttu-id="c8143-108">方法</span><span class="sxs-lookup"><span data-stu-id="c8143-108">Method</span></span>|<span data-ttu-id="c8143-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8143-109">Return Type</span></span>|<span data-ttu-id="c8143-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8143-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8143-111">列出 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="c8143-111">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="c8143-112">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c8143-112">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="c8143-113">列出[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8143-113">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="c8143-114">获取 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-114">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="c8143-115">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-115">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="c8143-116">读取[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8143-116">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="c8143-117">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-117">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="c8143-118">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-118">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="c8143-119">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8143-119">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="c8143-120">删除 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-120">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="c8143-121">无</span><span class="sxs-lookup"><span data-stu-id="c8143-121">None</span></span>|<span data-ttu-id="c8143-122">删除[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="c8143-122">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="c8143-123">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-123">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="c8143-124">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="c8143-124">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="c8143-125">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8143-125">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8143-126">属性</span><span class="sxs-lookup"><span data-stu-id="c8143-126">Properties</span></span>
|<span data-ttu-id="c8143-127">属性</span><span class="sxs-lookup"><span data-stu-id="c8143-127">Property</span></span>|<span data-ttu-id="c8143-128">类型</span><span class="sxs-lookup"><span data-stu-id="c8143-128">Type</span></span>|<span data-ttu-id="c8143-129">说明</span><span class="sxs-lookup"><span data-stu-id="c8143-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8143-130">id</span><span class="sxs-lookup"><span data-stu-id="c8143-130">id</span></span>|<span data-ttu-id="c8143-131">字符串</span><span class="sxs-lookup"><span data-stu-id="c8143-131">String</span></span>|<span data-ttu-id="c8143-132">Windows management 应用运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="c8143-132">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="c8143-133">healthState</span><span class="sxs-lookup"><span data-stu-id="c8143-133">healthState</span></span>|[<span data-ttu-id="c8143-134">healthState</span><span class="sxs-lookup"><span data-stu-id="c8143-134">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="c8143-135">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="c8143-135">Windows management app health state.</span></span> <span data-ttu-id="c8143-136">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="c8143-136">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="c8143-137">installedVersion</span><span class="sxs-lookup"><span data-stu-id="c8143-137">installedVersion</span></span>|<span data-ttu-id="c8143-138">字符串</span><span class="sxs-lookup"><span data-stu-id="c8143-138">String</span></span>|<span data-ttu-id="c8143-139">Windows 管理应用程序已安装版本。</span><span class="sxs-lookup"><span data-stu-id="c8143-139">Windows management app installed version.</span></span>|
|<span data-ttu-id="c8143-140">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="c8143-140">lastCheckInDateTime</span></span>|<span data-ttu-id="c8143-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8143-141">DateTimeOffset</span></span>|<span data-ttu-id="c8143-142">Windows 管理应用程序上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="c8143-142">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="c8143-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="c8143-143">deviceName</span></span>|<span data-ttu-id="c8143-144">String</span><span class="sxs-lookup"><span data-stu-id="c8143-144">String</span></span>|<span data-ttu-id="c8143-145">在其上安装 Windows management 应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c8143-145">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="c8143-146">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="c8143-146">deviceOSVersion</span></span>|<span data-ttu-id="c8143-147">字符串</span><span class="sxs-lookup"><span data-stu-id="c8143-147">String</span></span>|<span data-ttu-id="c8143-148">windows 10 OS 版本的 windows management app 安装在该设备上。</span><span class="sxs-lookup"><span data-stu-id="c8143-148">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8143-149">关系</span><span class="sxs-lookup"><span data-stu-id="c8143-149">Relationships</span></span>
<span data-ttu-id="c8143-150">无</span><span class="sxs-lookup"><span data-stu-id="c8143-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8143-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8143-151">JSON Representation</span></span>
<span data-ttu-id="c8143-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8143-152">Here is a JSON representation of the resource.</span></span>
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




