---
title: deviceAppManagement 资源类型
description: 充当所有设备应用管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 972590f5666f140e75074dd674433716961a17e7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752892"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="899bb-103">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="899bb-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="899bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="899bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="899bb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="899bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="899bb-106">充当所有设备应用管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="899bb-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="899bb-107">方法</span><span class="sxs-lookup"><span data-stu-id="899bb-107">Methods</span></span>
|<span data-ttu-id="899bb-108">方法</span><span class="sxs-lookup"><span data-stu-id="899bb-108">Method</span></span>|<span data-ttu-id="899bb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="899bb-109">Return Type</span></span>|<span data-ttu-id="899bb-110">说明</span><span class="sxs-lookup"><span data-stu-id="899bb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="899bb-111">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="899bb-111">Get deviceAppManagement</span></span>](../api/intune-books-deviceappmanagement-get.md)|[<span data-ttu-id="899bb-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="899bb-112">deviceAppManagement</span></span>](../resources/intune-books-deviceappmanagement.md)|<span data-ttu-id="899bb-113">读取 [deviceAppManagement](../resources/intune-books-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="899bb-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-books-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="899bb-114">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="899bb-114">Update deviceAppManagement</span></span>](../api/intune-books-deviceappmanagement-update.md)|[<span data-ttu-id="899bb-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="899bb-115">deviceAppManagement</span></span>](../resources/intune-books-deviceappmanagement.md)|<span data-ttu-id="899bb-116">更新 [deviceAppManagement](../resources/intune-books-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="899bb-116">Update the properties of a [deviceAppManagement](../resources/intune-books-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="899bb-117">属性</span><span class="sxs-lookup"><span data-stu-id="899bb-117">Properties</span></span>
|<span data-ttu-id="899bb-118">属性</span><span class="sxs-lookup"><span data-stu-id="899bb-118">Property</span></span>|<span data-ttu-id="899bb-119">类型</span><span class="sxs-lookup"><span data-stu-id="899bb-119">Type</span></span>|<span data-ttu-id="899bb-120">说明</span><span class="sxs-lookup"><span data-stu-id="899bb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="899bb-121">id</span><span class="sxs-lookup"><span data-stu-id="899bb-121">id</span></span>|<span data-ttu-id="899bb-122">String</span><span class="sxs-lookup"><span data-stu-id="899bb-122">String</span></span>|<span data-ttu-id="899bb-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="899bb-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="899bb-124">关系</span><span class="sxs-lookup"><span data-stu-id="899bb-124">Relationships</span></span>
|<span data-ttu-id="899bb-125">关系</span><span class="sxs-lookup"><span data-stu-id="899bb-125">Relationship</span></span>|<span data-ttu-id="899bb-126">类型</span><span class="sxs-lookup"><span data-stu-id="899bb-126">Type</span></span>|<span data-ttu-id="899bb-127">说明</span><span class="sxs-lookup"><span data-stu-id="899bb-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="899bb-128">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="899bb-128">managedEBooks</span></span>|<span data-ttu-id="899bb-129">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="899bb-129">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="899bb-130">托管的电子书。</span><span class="sxs-lookup"><span data-stu-id="899bb-130">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="899bb-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="899bb-131">JSON Representation</span></span>
<span data-ttu-id="899bb-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="899bb-132">Here is a JSON representation of the resource.</span></span>
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




