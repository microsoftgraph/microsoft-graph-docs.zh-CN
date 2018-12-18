---
title: windowsManagementAppHealthState 资源类型
description: Windows 管理应用程序运行状况状态实体。
author: tfitzmac
ms.openlocfilehash: 5ff77ce54a99ed71a8f4b3498a469342b2e46367
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359701"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="08aad-103">windowsManagementAppHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="08aad-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="08aad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08aad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08aad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08aad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08aad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="08aad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08aad-107">Windows 管理应用程序运行状况状态实体。</span><span class="sxs-lookup"><span data-stu-id="08aad-107">Windows management app health state entity.</span></span>
## <a name="methods"></a><span data-ttu-id="08aad-108">方法</span><span class="sxs-lookup"><span data-stu-id="08aad-108">Methods</span></span>
|<span data-ttu-id="08aad-109">方法</span><span class="sxs-lookup"><span data-stu-id="08aad-109">Method</span></span>|<span data-ttu-id="08aad-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="08aad-110">Return Type</span></span>|<span data-ttu-id="08aad-111">说明</span><span class="sxs-lookup"><span data-stu-id="08aad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08aad-112">列表 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="08aad-112">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="08aad-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="08aad-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="08aad-114">列出属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="08aad-114">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="08aad-115">获取 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-115">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="08aad-116">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-116">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="08aad-117">读取属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="08aad-117">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="08aad-118">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-118">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="08aad-119">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-119">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="08aad-120">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08aad-120">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="08aad-121">删除 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-121">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="08aad-122">无</span><span class="sxs-lookup"><span data-stu-id="08aad-122">None</span></span>|<span data-ttu-id="08aad-123">删除[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="08aad-123">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="08aad-124">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-124">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="08aad-125">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="08aad-125">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="08aad-126">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="08aad-126">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08aad-127">属性</span><span class="sxs-lookup"><span data-stu-id="08aad-127">Properties</span></span>
|<span data-ttu-id="08aad-128">属性</span><span class="sxs-lookup"><span data-stu-id="08aad-128">Property</span></span>|<span data-ttu-id="08aad-129">类型</span><span class="sxs-lookup"><span data-stu-id="08aad-129">Type</span></span>|<span data-ttu-id="08aad-130">说明</span><span class="sxs-lookup"><span data-stu-id="08aad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08aad-131">id</span><span class="sxs-lookup"><span data-stu-id="08aad-131">id</span></span>|<span data-ttu-id="08aad-132">字符串</span><span class="sxs-lookup"><span data-stu-id="08aad-132">String</span></span>|<span data-ttu-id="08aad-133">Windows 管理应用程序的运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="08aad-133">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="08aad-134">healthState</span><span class="sxs-lookup"><span data-stu-id="08aad-134">healthState</span></span>|[<span data-ttu-id="08aad-135">healthState</span><span class="sxs-lookup"><span data-stu-id="08aad-135">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="08aad-136">Windows 管理应用程序的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="08aad-136">Windows management app health state.</span></span> <span data-ttu-id="08aad-137">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="08aad-137">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="08aad-138">installedVersion</span><span class="sxs-lookup"><span data-stu-id="08aad-138">installedVersion</span></span>|<span data-ttu-id="08aad-139">字符串</span><span class="sxs-lookup"><span data-stu-id="08aad-139">String</span></span>|<span data-ttu-id="08aad-140">Windows 管理应用程序安装的版本。</span><span class="sxs-lookup"><span data-stu-id="08aad-140">Windows management app installed version.</span></span>|
|<span data-ttu-id="08aad-141">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="08aad-141">lastCheckInDateTime</span></span>|<span data-ttu-id="08aad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08aad-142">DateTimeOffset</span></span>|<span data-ttu-id="08aad-143">Windows 管理应用程序上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="08aad-143">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="08aad-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="08aad-144">deviceName</span></span>|<span data-ttu-id="08aad-145">String</span><span class="sxs-lookup"><span data-stu-id="08aad-145">String</span></span>|<span data-ttu-id="08aad-146">设备的 Windows 安装管理应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="08aad-146">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="08aad-147">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="08aad-147">deviceOSVersion</span></span>|<span data-ttu-id="08aad-148">字符串</span><span class="sxs-lookup"><span data-stu-id="08aad-148">String</span></span>|<span data-ttu-id="08aad-149">Windows 10 OS 版本的 Windows 安装管理应用程序的设备。</span><span class="sxs-lookup"><span data-stu-id="08aad-149">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08aad-150">Relationships</span><span class="sxs-lookup"><span data-stu-id="08aad-150">Relationships</span></span>
<span data-ttu-id="08aad-151">无</span><span class="sxs-lookup"><span data-stu-id="08aad-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08aad-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08aad-152">JSON Representation</span></span>
<span data-ttu-id="08aad-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08aad-153">Here is a JSON representation of the resource.</span></span>
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





