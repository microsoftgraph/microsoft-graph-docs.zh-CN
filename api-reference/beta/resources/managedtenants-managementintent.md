---
title: managementIntent 资源类型
description: 表示基线的元数据以及包含哪些管理模板。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7648da23e5d49a9bd2910c2ccbde7e676a1d7cd0
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402281"
---
# <a name="managementintent-resource-type"></a><span data-ttu-id="10055-103">managementIntent 资源类型</span><span class="sxs-lookup"><span data-stu-id="10055-103">managementIntent resource type</span></span>

<span data-ttu-id="10055-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="10055-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10055-105">表示基线的元数据以及包含哪些管理模板。</span><span class="sxs-lookup"><span data-stu-id="10055-105">Represents metadata for a baseline and what management templates are included.</span></span>

## <a name="methods"></a><span data-ttu-id="10055-106">方法</span><span class="sxs-lookup"><span data-stu-id="10055-106">Methods</span></span>
|<span data-ttu-id="10055-107">方法</span><span class="sxs-lookup"><span data-stu-id="10055-107">Method</span></span>|<span data-ttu-id="10055-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="10055-108">Return type</span></span>|<span data-ttu-id="10055-109">说明</span><span class="sxs-lookup"><span data-stu-id="10055-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10055-110">列出 managementIntents</span><span class="sxs-lookup"><span data-stu-id="10055-110">List managementIntents</span></span>](../api/managedtenants-managedtenant-list-managementintents.md)|<span data-ttu-id="10055-111">[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="10055-111">[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) collection</span></span>|<span data-ttu-id="10055-112">获取 [managementIntent 对象及其](../resources/managedtenants-managementintent.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="10055-112">Get a list of the [managementIntent](../resources/managedtenants-managementintent.md) objects and their properties.</span></span>|
|[<span data-ttu-id="10055-113">获取 managementIntent</span><span class="sxs-lookup"><span data-stu-id="10055-113">Get managementIntent</span></span>](../api/managedtenants-managementintent-get.md)|[<span data-ttu-id="10055-114">microsoft.graph.managedTenants.managementIntent</span><span class="sxs-lookup"><span data-stu-id="10055-114">microsoft.graph.managedTenants.managementIntent</span></span>](../resources/managedtenants-managementintent.md)|<span data-ttu-id="10055-115">读取 [managementIntent](../resources/managedtenants-managementintent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10055-115">Read the properties and relationships of a [managementIntent](../resources/managedtenants-managementintent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10055-116">属性</span><span class="sxs-lookup"><span data-stu-id="10055-116">Properties</span></span>
|<span data-ttu-id="10055-117">属性</span><span class="sxs-lookup"><span data-stu-id="10055-117">Property</span></span>|<span data-ttu-id="10055-118">类型</span><span class="sxs-lookup"><span data-stu-id="10055-118">Type</span></span>|<span data-ttu-id="10055-119">说明</span><span class="sxs-lookup"><span data-stu-id="10055-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10055-120">displayName</span><span class="sxs-lookup"><span data-stu-id="10055-120">displayName</span></span>|<span data-ttu-id="10055-121">String</span><span class="sxs-lookup"><span data-stu-id="10055-121">String</span></span>|<span data-ttu-id="10055-122">管理显示名称定义。</span><span class="sxs-lookup"><span data-stu-id="10055-122">The display name for the management intent.</span></span> <span data-ttu-id="10055-123">可选。</span><span class="sxs-lookup"><span data-stu-id="10055-123">Optional.</span></span> <span data-ttu-id="10055-124">只读。</span><span class="sxs-lookup"><span data-stu-id="10055-124">Read-only.</span></span>|
|<span data-ttu-id="10055-125">id</span><span class="sxs-lookup"><span data-stu-id="10055-125">id</span></span>|<span data-ttu-id="10055-126">String</span><span class="sxs-lookup"><span data-stu-id="10055-126">String</span></span>|<span data-ttu-id="10055-127">管理意图的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="10055-127">The unique identifier for the management intent.</span></span> <span data-ttu-id="10055-128">必填。</span><span class="sxs-lookup"><span data-stu-id="10055-128">Required.</span></span> <span data-ttu-id="10055-129">只读。</span><span class="sxs-lookup"><span data-stu-id="10055-129">Read-only.</span></span>|
|<span data-ttu-id="10055-130">isGlobal</span><span class="sxs-lookup"><span data-stu-id="10055-130">isGlobal</span></span>|<span data-ttu-id="10055-131">布尔</span><span class="sxs-lookup"><span data-stu-id="10055-131">Boolean</span></span>|<span data-ttu-id="10055-132">指示管理意图是否全局的标志。</span><span class="sxs-lookup"><span data-stu-id="10055-132">A flag indicating whether the management intent is global.</span></span> <span data-ttu-id="10055-133">必填。</span><span class="sxs-lookup"><span data-stu-id="10055-133">Required.</span></span> <span data-ttu-id="10055-134">只读。</span><span class="sxs-lookup"><span data-stu-id="10055-134">Read-only.</span></span>|
|<span data-ttu-id="10055-135">managementTemplates</span><span class="sxs-lookup"><span data-stu-id="10055-135">managementTemplates</span></span>|<span data-ttu-id="10055-136">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="10055-136">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) collection</span></span>|<span data-ttu-id="10055-137">与管理意图关联的管理模板的集合。</span><span class="sxs-lookup"><span data-stu-id="10055-137">The collection of management templates associated with the management intent.</span></span> <span data-ttu-id="10055-138">可选。</span><span class="sxs-lookup"><span data-stu-id="10055-138">Optional.</span></span> <span data-ttu-id="10055-139">只读。</span><span class="sxs-lookup"><span data-stu-id="10055-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10055-140">关系</span><span class="sxs-lookup"><span data-stu-id="10055-140">Relationships</span></span>
<span data-ttu-id="10055-141">无。</span><span class="sxs-lookup"><span data-stu-id="10055-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10055-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10055-142">JSON representation</span></span>
<span data-ttu-id="10055-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10055-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "isGlobal": "Boolean",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
