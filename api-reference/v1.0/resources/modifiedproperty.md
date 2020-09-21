---
title: modifiedProperty 资源类型
description: 指示 Azure AD 资源中已修改的所有属性，包括旧值和新值。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: d98d0aaa4850e8ef2b82f9f5deb17424c3ab98d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967378"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="f2cd5-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2cd5-103">modifiedProperty resource type</span></span>

<span data-ttu-id="f2cd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2cd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2cd5-105">指示 Azure AD 资源中已修改的所有属性，包括旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="f2cd5-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="f2cd5-106">属性</span><span class="sxs-lookup"><span data-stu-id="f2cd5-106">Properties</span></span>

| <span data-ttu-id="f2cd5-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2cd5-107">Property</span></span>     | <span data-ttu-id="f2cd5-108">类型</span><span class="sxs-lookup"><span data-stu-id="f2cd5-108">Type</span></span>   |<span data-ttu-id="f2cd5-109">说明</span><span class="sxs-lookup"><span data-stu-id="f2cd5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2cd5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f2cd5-110">displayName</span></span>|<span data-ttu-id="f2cd5-111">String</span><span class="sxs-lookup"><span data-stu-id="f2cd5-111">String</span></span>|<span data-ttu-id="f2cd5-112">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="f2cd5-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="f2cd5-113">NewValue</span><span class="sxs-lookup"><span data-stu-id="f2cd5-113">newValue</span></span>|<span data-ttu-id="f2cd5-114">String</span><span class="sxs-lookup"><span data-stu-id="f2cd5-114">String</span></span>|<span data-ttu-id="f2cd5-115">指示值的更新值。</span><span class="sxs-lookup"><span data-stu-id="f2cd5-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="f2cd5-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="f2cd5-116">oldValue</span></span>|<span data-ttu-id="f2cd5-117">String</span><span class="sxs-lookup"><span data-stu-id="f2cd5-117">String</span></span>|<span data-ttu-id="f2cd5-118">指示属性的 update) 之前 (以前的值。</span><span class="sxs-lookup"><span data-stu-id="f2cd5-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2cd5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2cd5-119">JSON representation</span></span>

<span data-ttu-id="f2cd5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2cd5-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

