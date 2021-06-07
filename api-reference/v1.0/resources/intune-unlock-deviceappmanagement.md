---
title: deviceAppManagement 资源类型
description: 充当所有设备和应用管理功能的容器的单一实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 238c5fbd6b4179dd0be320b5cf8cac6fd27eb9b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751832"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="cdb2f-103">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdb2f-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="cdb2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdb2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdb2f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdb2f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdb2f-106">充当所有设备和应用管理功能的容器的单一实体。</span><span class="sxs-lookup"><span data-stu-id="cdb2f-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="cdb2f-107">方法</span><span class="sxs-lookup"><span data-stu-id="cdb2f-107">Methods</span></span>
|<span data-ttu-id="cdb2f-108">方法</span><span class="sxs-lookup"><span data-stu-id="cdb2f-108">Method</span></span>|<span data-ttu-id="cdb2f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cdb2f-109">Return Type</span></span>|<span data-ttu-id="cdb2f-110">说明</span><span class="sxs-lookup"><span data-stu-id="cdb2f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cdb2f-111">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cdb2f-111">Get deviceAppManagement</span></span>](../api/intune-unlock-deviceappmanagement-get.md)|[<span data-ttu-id="cdb2f-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cdb2f-112">deviceAppManagement</span></span>](../resources/intune-unlock-deviceappmanagement.md)|<span data-ttu-id="cdb2f-113">读取 [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cdb2f-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="cdb2f-114">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cdb2f-114">Update deviceAppManagement</span></span>](../api/intune-unlock-deviceappmanagement-update.md)|[<span data-ttu-id="cdb2f-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cdb2f-115">deviceAppManagement</span></span>](../resources/intune-unlock-deviceappmanagement.md)|<span data-ttu-id="cdb2f-116">更新 [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cdb2f-116">Update the properties of a [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cdb2f-117">属性</span><span class="sxs-lookup"><span data-stu-id="cdb2f-117">Properties</span></span>
|<span data-ttu-id="cdb2f-118">属性</span><span class="sxs-lookup"><span data-stu-id="cdb2f-118">Property</span></span>|<span data-ttu-id="cdb2f-119">类型</span><span class="sxs-lookup"><span data-stu-id="cdb2f-119">Type</span></span>|<span data-ttu-id="cdb2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="cdb2f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdb2f-121">id</span><span class="sxs-lookup"><span data-stu-id="cdb2f-121">id</span></span>|<span data-ttu-id="cdb2f-122">String</span><span class="sxs-lookup"><span data-stu-id="cdb2f-122">String</span></span>|<span data-ttu-id="cdb2f-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cdb2f-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdb2f-124">关系</span><span class="sxs-lookup"><span data-stu-id="cdb2f-124">Relationships</span></span>
<span data-ttu-id="cdb2f-125">无</span><span class="sxs-lookup"><span data-stu-id="cdb2f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdb2f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdb2f-126">JSON Representation</span></span>
<span data-ttu-id="cdb2f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdb2f-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




