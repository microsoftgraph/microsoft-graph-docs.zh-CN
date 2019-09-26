---
title: windowsManagementAppHealthState 资源类型
description: Windows management 应用运行状况状态实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ffd7a970e36a93c93004e33ccdef2fefb782ed5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196656"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="84441-103">windowsManagementAppHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="84441-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="84441-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84441-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84441-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84441-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84441-106">Windows management 应用运行状况状态实体。</span><span class="sxs-lookup"><span data-stu-id="84441-106">Windows management app health state entity.</span></span>

## <a name="methods"></a><span data-ttu-id="84441-107">方法</span><span class="sxs-lookup"><span data-stu-id="84441-107">Methods</span></span>
|<span data-ttu-id="84441-108">方法</span><span class="sxs-lookup"><span data-stu-id="84441-108">Method</span></span>|<span data-ttu-id="84441-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="84441-109">Return Type</span></span>|<span data-ttu-id="84441-110">说明</span><span class="sxs-lookup"><span data-stu-id="84441-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84441-111">列出 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="84441-111">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="84441-112">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="84441-112">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="84441-113">列出[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84441-113">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="84441-114">获取 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-114">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="84441-115">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-115">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="84441-116">读取[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84441-116">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="84441-117">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-117">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="84441-118">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-118">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="84441-119">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84441-119">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="84441-120">删除 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-120">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="84441-121">无</span><span class="sxs-lookup"><span data-stu-id="84441-121">None</span></span>|<span data-ttu-id="84441-122">删除[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="84441-122">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="84441-123">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-123">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="84441-124">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="84441-124">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="84441-125">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84441-125">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84441-126">属性</span><span class="sxs-lookup"><span data-stu-id="84441-126">Properties</span></span>
|<span data-ttu-id="84441-127">属性</span><span class="sxs-lookup"><span data-stu-id="84441-127">Property</span></span>|<span data-ttu-id="84441-128">类型</span><span class="sxs-lookup"><span data-stu-id="84441-128">Type</span></span>|<span data-ttu-id="84441-129">说明</span><span class="sxs-lookup"><span data-stu-id="84441-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84441-130">id</span><span class="sxs-lookup"><span data-stu-id="84441-130">id</span></span>|<span data-ttu-id="84441-131">String</span><span class="sxs-lookup"><span data-stu-id="84441-131">String</span></span>|<span data-ttu-id="84441-132">Windows 管理应用运行状况状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="84441-132">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="84441-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="84441-133">This property is read-only.</span></span>|
|<span data-ttu-id="84441-134">healthState</span><span class="sxs-lookup"><span data-stu-id="84441-134">healthState</span></span>|[<span data-ttu-id="84441-135">healthState</span><span class="sxs-lookup"><span data-stu-id="84441-135">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="84441-136">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="84441-136">Windows management app health state.</span></span> <span data-ttu-id="84441-137">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="84441-137">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="84441-138">installedVersion</span><span class="sxs-lookup"><span data-stu-id="84441-138">installedVersion</span></span>|<span data-ttu-id="84441-139">String</span><span class="sxs-lookup"><span data-stu-id="84441-139">String</span></span>|<span data-ttu-id="84441-140">Windows 管理应用程序已安装版本。</span><span class="sxs-lookup"><span data-stu-id="84441-140">Windows management app installed version.</span></span>|
|<span data-ttu-id="84441-141">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="84441-141">lastCheckInDateTime</span></span>|<span data-ttu-id="84441-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84441-142">DateTimeOffset</span></span>|<span data-ttu-id="84441-143">Windows 管理应用程序上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="84441-143">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="84441-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="84441-144">deviceName</span></span>|<span data-ttu-id="84441-145">String</span><span class="sxs-lookup"><span data-stu-id="84441-145">String</span></span>|<span data-ttu-id="84441-146">在其上安装 Windows management 应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="84441-146">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="84441-147">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="84441-147">deviceOSVersion</span></span>|<span data-ttu-id="84441-148">String</span><span class="sxs-lookup"><span data-stu-id="84441-148">String</span></span>|<span data-ttu-id="84441-149">Windows 10 OS 版本的 Windows management app 安装在该设备上。</span><span class="sxs-lookup"><span data-stu-id="84441-149">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84441-150">关系</span><span class="sxs-lookup"><span data-stu-id="84441-150">Relationships</span></span>
<span data-ttu-id="84441-151">无</span><span class="sxs-lookup"><span data-stu-id="84441-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84441-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84441-152">JSON Representation</span></span>
<span data-ttu-id="84441-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84441-153">Here is a JSON representation of the resource.</span></span>
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



