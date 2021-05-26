---
title: windowsManagementApp 资源类型
description: Windows管理应用实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 540ba41779e64c57b5c74c7acf004172a1567c37
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665572"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="d261a-103">windowsManagementApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d261a-103">windowsManagementApp resource type</span></span>

<span data-ttu-id="d261a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d261a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d261a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d261a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d261a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d261a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d261a-107">Windows管理应用实体。</span><span class="sxs-lookup"><span data-stu-id="d261a-107">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d261a-108">方法</span><span class="sxs-lookup"><span data-stu-id="d261a-108">Methods</span></span>
|<span data-ttu-id="d261a-109">方法</span><span class="sxs-lookup"><span data-stu-id="d261a-109">Method</span></span>|<span data-ttu-id="d261a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d261a-110">Return Type</span></span>|<span data-ttu-id="d261a-111">说明</span><span class="sxs-lookup"><span data-stu-id="d261a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d261a-112">获取 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d261a-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="d261a-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d261a-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="d261a-114">读取 [windowsManagementApp 对象的属性和](../resources/intune-devices-windowsmanagementapp.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d261a-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="d261a-115">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d261a-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="d261a-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d261a-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="d261a-117">更新 [windowsManagementApp 对象](../resources/intune-devices-windowsmanagementapp.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d261a-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="d261a-118">setAsManagedInstaller 操作</span><span class="sxs-lookup"><span data-stu-id="d261a-118">setAsManagedInstaller action</span></span>](../api/intune-devices-windowsmanagementapp-setasmanagedinstaller.md)|<span data-ttu-id="d261a-119">无</span><span class="sxs-lookup"><span data-stu-id="d261a-119">None</span></span>|<span data-ttu-id="d261a-120">设置呼叫者租户的托管安装程序状态</span><span class="sxs-lookup"><span data-stu-id="d261a-120">Set the Managed Installer status for the caller tenant</span></span>|

## <a name="properties"></a><span data-ttu-id="d261a-121">属性</span><span class="sxs-lookup"><span data-stu-id="d261a-121">Properties</span></span>
|<span data-ttu-id="d261a-122">属性</span><span class="sxs-lookup"><span data-stu-id="d261a-122">Property</span></span>|<span data-ttu-id="d261a-123">类型</span><span class="sxs-lookup"><span data-stu-id="d261a-123">Type</span></span>|<span data-ttu-id="d261a-124">说明</span><span class="sxs-lookup"><span data-stu-id="d261a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d261a-125">id</span><span class="sxs-lookup"><span data-stu-id="d261a-125">id</span></span>|<span data-ttu-id="d261a-126">String</span><span class="sxs-lookup"><span data-stu-id="d261a-126">String</span></span>|<span data-ttu-id="d261a-127">管理应用程序的唯Windows标识符</span><span class="sxs-lookup"><span data-stu-id="d261a-127">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="d261a-128">availableVersion</span><span class="sxs-lookup"><span data-stu-id="d261a-128">availableVersion</span></span>|<span data-ttu-id="d261a-129">String</span><span class="sxs-lookup"><span data-stu-id="d261a-129">String</span></span>|<span data-ttu-id="d261a-130">Windows管理应用可用版本。</span><span class="sxs-lookup"><span data-stu-id="d261a-130">Windows management app available version.</span></span>|
|<span data-ttu-id="d261a-131">managedInstaller</span><span class="sxs-lookup"><span data-stu-id="d261a-131">managedInstaller</span></span>|[<span data-ttu-id="d261a-132">managedInstallerStatus</span><span class="sxs-lookup"><span data-stu-id="d261a-132">managedInstallerStatus</span></span>](../resources/intune-devices-managedinstallerstatus.md)|<span data-ttu-id="d261a-133">托管安装程序状态。</span><span class="sxs-lookup"><span data-stu-id="d261a-133">Managed Installer Status.</span></span> <span data-ttu-id="d261a-134">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="d261a-134">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d261a-135">managedInstallerConfiguredDateTime</span><span class="sxs-lookup"><span data-stu-id="d261a-135">managedInstallerConfiguredDateTime</span></span>|<span data-ttu-id="d261a-136">String</span><span class="sxs-lookup"><span data-stu-id="d261a-136">String</span></span>|<span data-ttu-id="d261a-137">托管安装程序配置的日期时间</span><span class="sxs-lookup"><span data-stu-id="d261a-137">Managed Installer Configured Date Time</span></span>|

## <a name="relationships"></a><span data-ttu-id="d261a-138">关系</span><span class="sxs-lookup"><span data-stu-id="d261a-138">Relationships</span></span>
|<span data-ttu-id="d261a-139">关系</span><span class="sxs-lookup"><span data-stu-id="d261a-139">Relationship</span></span>|<span data-ttu-id="d261a-140">类型</span><span class="sxs-lookup"><span data-stu-id="d261a-140">Type</span></span>|<span data-ttu-id="d261a-141">说明</span><span class="sxs-lookup"><span data-stu-id="d261a-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d261a-142">healthStates</span><span class="sxs-lookup"><span data-stu-id="d261a-142">healthStates</span></span>|<span data-ttu-id="d261a-143">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d261a-143">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="d261a-144">已安装的运行状况状态列表Windows管理应用。</span><span class="sxs-lookup"><span data-stu-id="d261a-144">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d261a-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d261a-145">JSON Representation</span></span>
<span data-ttu-id="d261a-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d261a-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String",
  "managedInstaller": "String",
  "managedInstallerConfiguredDateTime": "String"
}
```




