---
title: windowsManagementAppHealthState 资源类型
description: Windows management 应用运行状况状态实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4cf9c680e929e06abce33b96fb89b232dc928ac
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731041"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="1495c-103">windowsManagementAppHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="1495c-103">windowsManagementAppHealthState resource type</span></span>

<span data-ttu-id="1495c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1495c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1495c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1495c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1495c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1495c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1495c-107">Windows management 应用运行状况状态实体。</span><span class="sxs-lookup"><span data-stu-id="1495c-107">Windows management app health state entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1495c-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1495c-108">Methods</span></span>
|<span data-ttu-id="1495c-109">方法</span><span class="sxs-lookup"><span data-stu-id="1495c-109">Method</span></span>|<span data-ttu-id="1495c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1495c-110">Return Type</span></span>|<span data-ttu-id="1495c-111">说明</span><span class="sxs-lookup"><span data-stu-id="1495c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1495c-112">列出 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="1495c-112">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="1495c-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1495c-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="1495c-114">列出 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1495c-114">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="1495c-115">获取 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-115">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="1495c-116">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-116">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="1495c-117">读取 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1495c-117">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="1495c-118">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-118">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="1495c-119">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-119">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="1495c-120">创建新的 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1495c-120">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="1495c-121">删除 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-121">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="1495c-122">无</span><span class="sxs-lookup"><span data-stu-id="1495c-122">None</span></span>|<span data-ttu-id="1495c-123">删除 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="1495c-123">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="1495c-124">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-124">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="1495c-125">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="1495c-125">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="1495c-126">更新 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1495c-126">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1495c-127">属性</span><span class="sxs-lookup"><span data-stu-id="1495c-127">Properties</span></span>
|<span data-ttu-id="1495c-128">属性</span><span class="sxs-lookup"><span data-stu-id="1495c-128">Property</span></span>|<span data-ttu-id="1495c-129">类型</span><span class="sxs-lookup"><span data-stu-id="1495c-129">Type</span></span>|<span data-ttu-id="1495c-130">说明</span><span class="sxs-lookup"><span data-stu-id="1495c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1495c-131">id</span><span class="sxs-lookup"><span data-stu-id="1495c-131">id</span></span>|<span data-ttu-id="1495c-132">String</span><span class="sxs-lookup"><span data-stu-id="1495c-132">String</span></span>|<span data-ttu-id="1495c-133">Windows 管理应用运行状况状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1495c-133">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="1495c-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1495c-134">This property is read-only.</span></span>|
|<span data-ttu-id="1495c-135">healthState</span><span class="sxs-lookup"><span data-stu-id="1495c-135">healthState</span></span>|[<span data-ttu-id="1495c-136">healthState</span><span class="sxs-lookup"><span data-stu-id="1495c-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="1495c-137">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="1495c-137">Windows management app health state.</span></span> <span data-ttu-id="1495c-138">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="1495c-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="1495c-139">installedVersion</span><span class="sxs-lookup"><span data-stu-id="1495c-139">installedVersion</span></span>|<span data-ttu-id="1495c-140">String</span><span class="sxs-lookup"><span data-stu-id="1495c-140">String</span></span>|<span data-ttu-id="1495c-141">Windows 管理应用程序已安装版本。</span><span class="sxs-lookup"><span data-stu-id="1495c-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="1495c-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="1495c-142">lastCheckInDateTime</span></span>|<span data-ttu-id="1495c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1495c-143">DateTimeOffset</span></span>|<span data-ttu-id="1495c-144">Windows 管理应用程序上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="1495c-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="1495c-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="1495c-145">deviceName</span></span>|<span data-ttu-id="1495c-146">String</span><span class="sxs-lookup"><span data-stu-id="1495c-146">String</span></span>|<span data-ttu-id="1495c-147">在其上安装 Windows management 应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="1495c-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="1495c-148">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="1495c-148">deviceOSVersion</span></span>|<span data-ttu-id="1495c-149">String</span><span class="sxs-lookup"><span data-stu-id="1495c-149">String</span></span>|<span data-ttu-id="1495c-150">Windows 10 OS 版本的 Windows management app 安装在该设备上。</span><span class="sxs-lookup"><span data-stu-id="1495c-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1495c-151">关系</span><span class="sxs-lookup"><span data-stu-id="1495c-151">Relationships</span></span>
<span data-ttu-id="1495c-152">无</span><span class="sxs-lookup"><span data-stu-id="1495c-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1495c-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1495c-153">JSON Representation</span></span>
<span data-ttu-id="1495c-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1495c-154">Here is a JSON representation of the resource.</span></span>
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





