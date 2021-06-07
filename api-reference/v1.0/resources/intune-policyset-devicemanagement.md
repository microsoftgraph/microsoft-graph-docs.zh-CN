---
title: deviceManagement 资源类型
description: 充当所有设备和应用管理功能的容器的单一实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bfc2ddb9f3883f2157a451edc53ea4b33590371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751824"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="6d0a5-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d0a5-103">deviceManagement resource type</span></span>

<span data-ttu-id="6d0a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d0a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d0a5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d0a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d0a5-106">充当所有设备和应用管理功能的容器的单一实体。</span><span class="sxs-lookup"><span data-stu-id="6d0a5-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="6d0a5-107">方法</span><span class="sxs-lookup"><span data-stu-id="6d0a5-107">Methods</span></span>
|<span data-ttu-id="6d0a5-108">方法</span><span class="sxs-lookup"><span data-stu-id="6d0a5-108">Method</span></span>|<span data-ttu-id="6d0a5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6d0a5-109">Return Type</span></span>|<span data-ttu-id="6d0a5-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d0a5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d0a5-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6d0a5-111">Get deviceManagement</span></span>](../api/intune-policyset-devicemanagement-get.md)|[<span data-ttu-id="6d0a5-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6d0a5-112">deviceManagement</span></span>](../resources/intune-policyset-devicemanagement.md)|<span data-ttu-id="6d0a5-113">读取 [deviceManagement](../resources/intune-policyset-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d0a5-113">Read properties and relationships of the [deviceManagement](../resources/intune-policyset-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="6d0a5-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6d0a5-114">Update deviceManagement</span></span>](../api/intune-policyset-devicemanagement-update.md)|[<span data-ttu-id="6d0a5-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6d0a5-115">deviceManagement</span></span>](../resources/intune-policyset-devicemanagement.md)|<span data-ttu-id="6d0a5-116">更新 [deviceManagement](../resources/intune-policyset-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6d0a5-116">Update the properties of a [deviceManagement](../resources/intune-policyset-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d0a5-117">属性</span><span class="sxs-lookup"><span data-stu-id="6d0a5-117">Properties</span></span>
|<span data-ttu-id="6d0a5-118">属性</span><span class="sxs-lookup"><span data-stu-id="6d0a5-118">Property</span></span>|<span data-ttu-id="6d0a5-119">类型</span><span class="sxs-lookup"><span data-stu-id="6d0a5-119">Type</span></span>|<span data-ttu-id="6d0a5-120">说明</span><span class="sxs-lookup"><span data-stu-id="6d0a5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d0a5-121">id</span><span class="sxs-lookup"><span data-stu-id="6d0a5-121">id</span></span>|<span data-ttu-id="6d0a5-122">String</span><span class="sxs-lookup"><span data-stu-id="6d0a5-122">String</span></span>|<span data-ttu-id="6d0a5-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6d0a5-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d0a5-124">关系</span><span class="sxs-lookup"><span data-stu-id="6d0a5-124">Relationships</span></span>
<span data-ttu-id="6d0a5-125">无</span><span class="sxs-lookup"><span data-stu-id="6d0a5-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d0a5-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d0a5-126">JSON Representation</span></span>
<span data-ttu-id="6d0a5-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d0a5-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




