---
title: 设置资源类型
description: 表示在基线中使用的设置。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2545dc6aa11668359fa9dda636412d36f8d92de1
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402397"
---
# <a name="setting-resource-type"></a><span data-ttu-id="5722b-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="5722b-103">setting resource type</span></span>

<span data-ttu-id="5722b-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5722b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5722b-105">表示在基线中使用的设置。</span><span class="sxs-lookup"><span data-stu-id="5722b-105">Represents a setting that is used within a baseline.</span></span>

## <a name="properties"></a><span data-ttu-id="5722b-106">属性</span><span class="sxs-lookup"><span data-stu-id="5722b-106">Properties</span></span>
|<span data-ttu-id="5722b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5722b-107">Property</span></span>|<span data-ttu-id="5722b-108">类型</span><span class="sxs-lookup"><span data-stu-id="5722b-108">Type</span></span>|<span data-ttu-id="5722b-109">说明</span><span class="sxs-lookup"><span data-stu-id="5722b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5722b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5722b-110">displayName</span></span>|<span data-ttu-id="5722b-111">String</span><span class="sxs-lookup"><span data-stu-id="5722b-111">String</span></span>|<span data-ttu-id="5722b-112">设置显示名称值。</span><span class="sxs-lookup"><span data-stu-id="5722b-112">The display name for the setting.</span></span> <span data-ttu-id="5722b-113">必填。</span><span class="sxs-lookup"><span data-stu-id="5722b-113">Required.</span></span> <span data-ttu-id="5722b-114">只读。</span><span class="sxs-lookup"><span data-stu-id="5722b-114">Read-only.</span></span>|
|<span data-ttu-id="5722b-115">jsonValue</span><span class="sxs-lookup"><span data-stu-id="5722b-115">jsonValue</span></span>|<span data-ttu-id="5722b-116">String</span><span class="sxs-lookup"><span data-stu-id="5722b-116">String</span></span>|<span data-ttu-id="5722b-117">设置为 JSON 字符串序列化的设置的值。</span><span class="sxs-lookup"><span data-stu-id="5722b-117">The value for the setting serialized as string of JSON.</span></span> <span data-ttu-id="5722b-118">必填。</span><span class="sxs-lookup"><span data-stu-id="5722b-118">Required.</span></span> <span data-ttu-id="5722b-119">只读。</span><span class="sxs-lookup"><span data-stu-id="5722b-119">Read-only.</span></span>|
|<span data-ttu-id="5722b-120">overwriteAllowed</span><span class="sxs-lookup"><span data-stu-id="5722b-120">overwriteAllowed</span></span>|<span data-ttu-id="5722b-121">布尔</span><span class="sxs-lookup"><span data-stu-id="5722b-121">Boolean</span></span>|<span data-ttu-id="5722b-122">指示应用此设置时是否可以替代现有配置的标志。</span><span class="sxs-lookup"><span data-stu-id="5722b-122">A flag indicating whether the setting can be override existing configurations when applied.</span></span> <span data-ttu-id="5722b-123">必填。</span><span class="sxs-lookup"><span data-stu-id="5722b-123">Required.</span></span> <span data-ttu-id="5722b-124">只读。</span><span class="sxs-lookup"><span data-stu-id="5722b-124">Read-only.</span></span>|
|<span data-ttu-id="5722b-125">valueType</span><span class="sxs-lookup"><span data-stu-id="5722b-125">valueType</span></span>|<span data-ttu-id="5722b-126">managementParameterValueType</span><span class="sxs-lookup"><span data-stu-id="5722b-126">managementParameterValueType</span></span>|<span data-ttu-id="5722b-127">设置数据类型值。</span><span class="sxs-lookup"><span data-stu-id="5722b-127">The data type for the setting.</span></span> <span data-ttu-id="5722b-128">可取值为：`string`、`integer`、`boolean`、`guid`、`stringCollection`、`integerCollection`、`booleanCollection`、`guidCollection`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5722b-128">Possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span></span> <span data-ttu-id="5722b-129">必填。</span><span class="sxs-lookup"><span data-stu-id="5722b-129">Required.</span></span> <span data-ttu-id="5722b-130">只读。</span><span class="sxs-lookup"><span data-stu-id="5722b-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5722b-131">关系</span><span class="sxs-lookup"><span data-stu-id="5722b-131">Relationships</span></span>
<span data-ttu-id="5722b-132">无。</span><span class="sxs-lookup"><span data-stu-id="5722b-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5722b-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5722b-133">JSON representation</span></span>
<span data-ttu-id="5722b-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5722b-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```
