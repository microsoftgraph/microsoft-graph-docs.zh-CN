---
title: deviceAppManagement 资源类型
description: 充当所有设备和应用管理功能的容器的单一实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 783ba507373c90cee6ba3e646d085f1a6502c5cf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751825"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="cddcb-103">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="cddcb-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="cddcb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cddcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cddcb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cddcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cddcb-106">充当所有设备和应用管理功能的容器的单一实体。</span><span class="sxs-lookup"><span data-stu-id="cddcb-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="cddcb-107">方法</span><span class="sxs-lookup"><span data-stu-id="cddcb-107">Methods</span></span>
|<span data-ttu-id="cddcb-108">方法</span><span class="sxs-lookup"><span data-stu-id="cddcb-108">Method</span></span>|<span data-ttu-id="cddcb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cddcb-109">Return Type</span></span>|<span data-ttu-id="cddcb-110">说明</span><span class="sxs-lookup"><span data-stu-id="cddcb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cddcb-111">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cddcb-111">Get deviceAppManagement</span></span>](../api/intune-policyset-deviceappmanagement-get.md)|[<span data-ttu-id="cddcb-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cddcb-112">deviceAppManagement</span></span>](../resources/intune-policyset-deviceappmanagement.md)|<span data-ttu-id="cddcb-113">读取 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cddcb-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="cddcb-114">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cddcb-114">Update deviceAppManagement</span></span>](../api/intune-policyset-deviceappmanagement-update.md)|[<span data-ttu-id="cddcb-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cddcb-115">deviceAppManagement</span></span>](../resources/intune-policyset-deviceappmanagement.md)|<span data-ttu-id="cddcb-116">更新 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cddcb-116">Update the properties of a [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cddcb-117">属性</span><span class="sxs-lookup"><span data-stu-id="cddcb-117">Properties</span></span>
|<span data-ttu-id="cddcb-118">属性</span><span class="sxs-lookup"><span data-stu-id="cddcb-118">Property</span></span>|<span data-ttu-id="cddcb-119">类型</span><span class="sxs-lookup"><span data-stu-id="cddcb-119">Type</span></span>|<span data-ttu-id="cddcb-120">说明</span><span class="sxs-lookup"><span data-stu-id="cddcb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cddcb-121">id</span><span class="sxs-lookup"><span data-stu-id="cddcb-121">id</span></span>|<span data-ttu-id="cddcb-122">String</span><span class="sxs-lookup"><span data-stu-id="cddcb-122">String</span></span>|<span data-ttu-id="cddcb-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cddcb-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cddcb-124">关系</span><span class="sxs-lookup"><span data-stu-id="cddcb-124">Relationships</span></span>
<span data-ttu-id="cddcb-125">无</span><span class="sxs-lookup"><span data-stu-id="cddcb-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cddcb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cddcb-126">JSON Representation</span></span>
<span data-ttu-id="cddcb-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cddcb-127">Here is a JSON representation of the resource.</span></span>
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




