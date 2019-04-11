---
title: windowsManagementApp 资源类型
description: Windows 管理应用实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99367ae51bbfe2ad044a99b465f70f5f8316e2d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802420"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="c5249-103">windowsManagementApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5249-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="c5249-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5249-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5249-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5249-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5249-106">Windows 管理应用实体。</span><span class="sxs-lookup"><span data-stu-id="c5249-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c5249-107">方法</span><span class="sxs-lookup"><span data-stu-id="c5249-107">Methods</span></span>
|<span data-ttu-id="c5249-108">方法</span><span class="sxs-lookup"><span data-stu-id="c5249-108">Method</span></span>|<span data-ttu-id="c5249-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5249-109">Return Type</span></span>|<span data-ttu-id="c5249-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5249-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5249-111">获取 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="c5249-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="c5249-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="c5249-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="c5249-113">读取[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5249-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="c5249-114">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="c5249-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="c5249-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="c5249-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="c5249-116">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5249-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5249-117">属性</span><span class="sxs-lookup"><span data-stu-id="c5249-117">Properties</span></span>
|<span data-ttu-id="c5249-118">属性</span><span class="sxs-lookup"><span data-stu-id="c5249-118">Property</span></span>|<span data-ttu-id="c5249-119">类型</span><span class="sxs-lookup"><span data-stu-id="c5249-119">Type</span></span>|<span data-ttu-id="c5249-120">说明</span><span class="sxs-lookup"><span data-stu-id="c5249-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5249-121">id</span><span class="sxs-lookup"><span data-stu-id="c5249-121">id</span></span>|<span data-ttu-id="c5249-122">String</span><span class="sxs-lookup"><span data-stu-id="c5249-122">String</span></span>|<span data-ttu-id="c5249-123">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="c5249-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="c5249-124">availableVersion</span><span class="sxs-lookup"><span data-stu-id="c5249-124">availableVersion</span></span>|<span data-ttu-id="c5249-125">String</span><span class="sxs-lookup"><span data-stu-id="c5249-125">String</span></span>|<span data-ttu-id="c5249-126">Windows 管理应用程序的可用版本。</span><span class="sxs-lookup"><span data-stu-id="c5249-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5249-127">关系</span><span class="sxs-lookup"><span data-stu-id="c5249-127">Relationships</span></span>
|<span data-ttu-id="c5249-128">关系</span><span class="sxs-lookup"><span data-stu-id="c5249-128">Relationship</span></span>|<span data-ttu-id="c5249-129">类型</span><span class="sxs-lookup"><span data-stu-id="c5249-129">Type</span></span>|<span data-ttu-id="c5249-130">说明</span><span class="sxs-lookup"><span data-stu-id="c5249-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5249-131">healthSummary</span><span class="sxs-lookup"><span data-stu-id="c5249-131">healthSummary</span></span>|[<span data-ttu-id="c5249-132">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="c5249-132">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="c5249-133">Windows management 应用的运行状况摘要。</span><span class="sxs-lookup"><span data-stu-id="c5249-133">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="c5249-134">healthStates</span><span class="sxs-lookup"><span data-stu-id="c5249-134">healthStates</span></span>|<span data-ttu-id="c5249-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5249-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="c5249-136">已安装的 Windows management 应用的运行状况状态列表。</span><span class="sxs-lookup"><span data-stu-id="c5249-136">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5249-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5249-137">JSON Representation</span></span>
<span data-ttu-id="c5249-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5249-138">Here is a JSON representation of the resource.</span></span>
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
  "availableVersion": "String"
}
```





