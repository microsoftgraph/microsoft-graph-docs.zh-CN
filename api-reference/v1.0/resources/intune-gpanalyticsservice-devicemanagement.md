---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 78034b4c466ef534cc92ebed6157e80a7c7ed2f7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755231"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="a27fa-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a27fa-103">deviceManagement resource type</span></span>

<span data-ttu-id="a27fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a27fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a27fa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a27fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a27fa-106">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="a27fa-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="a27fa-107">方法</span><span class="sxs-lookup"><span data-stu-id="a27fa-107">Methods</span></span>
|<span data-ttu-id="a27fa-108">方法</span><span class="sxs-lookup"><span data-stu-id="a27fa-108">Method</span></span>|<span data-ttu-id="a27fa-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a27fa-109">Return Type</span></span>|<span data-ttu-id="a27fa-110">说明</span><span class="sxs-lookup"><span data-stu-id="a27fa-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a27fa-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a27fa-111">Get deviceManagement</span></span>](../api/intune-gpanalyticsservice-devicemanagement-get.md)|[<span data-ttu-id="a27fa-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a27fa-112">deviceManagement</span></span>](../resources/intune-gpanalyticsservice-devicemanagement.md)|<span data-ttu-id="a27fa-113">读取 [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a27fa-113">Read properties and relationships of the [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="a27fa-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a27fa-114">Update deviceManagement</span></span>](../api/intune-gpanalyticsservice-devicemanagement-update.md)|[<span data-ttu-id="a27fa-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a27fa-115">deviceManagement</span></span>](../resources/intune-gpanalyticsservice-devicemanagement.md)|<span data-ttu-id="a27fa-116">更新 [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a27fa-116">Update the properties of a [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a27fa-117">属性</span><span class="sxs-lookup"><span data-stu-id="a27fa-117">Properties</span></span>
|<span data-ttu-id="a27fa-118">属性</span><span class="sxs-lookup"><span data-stu-id="a27fa-118">Property</span></span>|<span data-ttu-id="a27fa-119">类型</span><span class="sxs-lookup"><span data-stu-id="a27fa-119">Type</span></span>|<span data-ttu-id="a27fa-120">说明</span><span class="sxs-lookup"><span data-stu-id="a27fa-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a27fa-121">id</span><span class="sxs-lookup"><span data-stu-id="a27fa-121">id</span></span>|<span data-ttu-id="a27fa-122">String</span><span class="sxs-lookup"><span data-stu-id="a27fa-122">String</span></span>|<span data-ttu-id="a27fa-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a27fa-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="a27fa-124">关系</span><span class="sxs-lookup"><span data-stu-id="a27fa-124">Relationships</span></span>
<span data-ttu-id="a27fa-125">无</span><span class="sxs-lookup"><span data-stu-id="a27fa-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a27fa-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a27fa-126">JSON Representation</span></span>
<span data-ttu-id="a27fa-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a27fa-127">Here is a JSON representation of the resource.</span></span>
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




