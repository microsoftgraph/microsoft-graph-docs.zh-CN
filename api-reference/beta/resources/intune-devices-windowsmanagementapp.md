---
title: windowsManagementApp 资源类型
description: Windows 管理应用实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4525767a81b0e69ed1c99ae4b1a20051304cf1f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941908"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="9b39a-103">windowsManagementApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b39a-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="9b39a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b39a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b39a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b39a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b39a-106">Windows 管理应用实体。</span><span class="sxs-lookup"><span data-stu-id="9b39a-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="9b39a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9b39a-107">Methods</span></span>
|<span data-ttu-id="9b39a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9b39a-108">Method</span></span>|<span data-ttu-id="9b39a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9b39a-109">Return Type</span></span>|<span data-ttu-id="9b39a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b39a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b39a-111">获取 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="9b39a-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="9b39a-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="9b39a-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="9b39a-113">读取[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9b39a-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="9b39a-114">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="9b39a-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="9b39a-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="9b39a-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="9b39a-116">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b39a-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b39a-117">属性</span><span class="sxs-lookup"><span data-stu-id="9b39a-117">Properties</span></span>
|<span data-ttu-id="9b39a-118">属性</span><span class="sxs-lookup"><span data-stu-id="9b39a-118">Property</span></span>|<span data-ttu-id="9b39a-119">类型</span><span class="sxs-lookup"><span data-stu-id="9b39a-119">Type</span></span>|<span data-ttu-id="9b39a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b39a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b39a-121">id</span><span class="sxs-lookup"><span data-stu-id="9b39a-121">id</span></span>|<span data-ttu-id="9b39a-122">String</span><span class="sxs-lookup"><span data-stu-id="9b39a-122">String</span></span>|<span data-ttu-id="9b39a-123">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="9b39a-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="9b39a-124">availableVersion</span><span class="sxs-lookup"><span data-stu-id="9b39a-124">availableVersion</span></span>|<span data-ttu-id="9b39a-125">String</span><span class="sxs-lookup"><span data-stu-id="9b39a-125">String</span></span>|<span data-ttu-id="9b39a-126">Windows 管理应用程序的可用版本。</span><span class="sxs-lookup"><span data-stu-id="9b39a-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b39a-127">关系</span><span class="sxs-lookup"><span data-stu-id="9b39a-127">Relationships</span></span>
|<span data-ttu-id="9b39a-128">关系</span><span class="sxs-lookup"><span data-stu-id="9b39a-128">Relationship</span></span>|<span data-ttu-id="9b39a-129">类型</span><span class="sxs-lookup"><span data-stu-id="9b39a-129">Type</span></span>|<span data-ttu-id="9b39a-130">说明</span><span class="sxs-lookup"><span data-stu-id="9b39a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b39a-131">healthSummary</span><span class="sxs-lookup"><span data-stu-id="9b39a-131">healthSummary</span></span>|[<span data-ttu-id="9b39a-132">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9b39a-132">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="9b39a-133">Windows management 应用的运行状况摘要。</span><span class="sxs-lookup"><span data-stu-id="9b39a-133">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="9b39a-134">healthStates</span><span class="sxs-lookup"><span data-stu-id="9b39a-134">healthStates</span></span>|<span data-ttu-id="9b39a-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="9b39a-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="9b39a-136">已安装的 Windows management 应用的运行状况状态列表。</span><span class="sxs-lookup"><span data-stu-id="9b39a-136">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b39a-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b39a-137">JSON Representation</span></span>
<span data-ttu-id="9b39a-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b39a-138">Here is a JSON representation of the resource.</span></span>
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




