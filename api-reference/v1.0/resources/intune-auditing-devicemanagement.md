---
title: deviceManagement 资源类型
description: 充当所有设备应用管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b55c85abc632b149a4e397c007a4c7d4b79a6c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752893"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="4b31d-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b31d-103">deviceManagement resource type</span></span>

<span data-ttu-id="4b31d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b31d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b31d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b31d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b31d-106">充当所有设备应用管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="4b31d-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="4b31d-107">方法</span><span class="sxs-lookup"><span data-stu-id="4b31d-107">Methods</span></span>
|<span data-ttu-id="4b31d-108">方法</span><span class="sxs-lookup"><span data-stu-id="4b31d-108">Method</span></span>|<span data-ttu-id="4b31d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b31d-109">Return Type</span></span>|<span data-ttu-id="4b31d-110">说明</span><span class="sxs-lookup"><span data-stu-id="4b31d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b31d-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4b31d-111">Get deviceManagement</span></span>](../api/intune-auditing-devicemanagement-get.md)|[<span data-ttu-id="4b31d-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4b31d-112">deviceManagement</span></span>](../resources/intune-auditing-devicemanagement.md)|<span data-ttu-id="4b31d-113">读取 [deviceManagement](../resources/intune-auditing-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b31d-113">Read properties and relationships of the [deviceManagement](../resources/intune-auditing-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="4b31d-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4b31d-114">Update deviceManagement</span></span>](../api/intune-auditing-devicemanagement-update.md)|[<span data-ttu-id="4b31d-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4b31d-115">deviceManagement</span></span>](../resources/intune-auditing-devicemanagement.md)|<span data-ttu-id="4b31d-116">更新 [deviceManagement](../resources/intune-auditing-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4b31d-116">Update the properties of a [deviceManagement](../resources/intune-auditing-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b31d-117">属性</span><span class="sxs-lookup"><span data-stu-id="4b31d-117">Properties</span></span>
|<span data-ttu-id="4b31d-118">属性</span><span class="sxs-lookup"><span data-stu-id="4b31d-118">Property</span></span>|<span data-ttu-id="4b31d-119">类型</span><span class="sxs-lookup"><span data-stu-id="4b31d-119">Type</span></span>|<span data-ttu-id="4b31d-120">说明</span><span class="sxs-lookup"><span data-stu-id="4b31d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b31d-121">id</span><span class="sxs-lookup"><span data-stu-id="4b31d-121">id</span></span>|<span data-ttu-id="4b31d-122">String</span><span class="sxs-lookup"><span data-stu-id="4b31d-122">String</span></span>|<span data-ttu-id="4b31d-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4b31d-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b31d-124">关系</span><span class="sxs-lookup"><span data-stu-id="4b31d-124">Relationships</span></span>
|<span data-ttu-id="4b31d-125">关系</span><span class="sxs-lookup"><span data-stu-id="4b31d-125">Relationship</span></span>|<span data-ttu-id="4b31d-126">类型</span><span class="sxs-lookup"><span data-stu-id="4b31d-126">Type</span></span>|<span data-ttu-id="4b31d-127">说明</span><span class="sxs-lookup"><span data-stu-id="4b31d-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b31d-128">auditEvents</span><span class="sxs-lookup"><span data-stu-id="4b31d-128">auditEvents</span></span>|<span data-ttu-id="4b31d-129">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b31d-129">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="4b31d-130">审核事件</span><span class="sxs-lookup"><span data-stu-id="4b31d-130">The Audit Events</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b31d-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b31d-131">JSON Representation</span></span>
<span data-ttu-id="4b31d-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b31d-132">Here is a JSON representation of the resource.</span></span>
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




