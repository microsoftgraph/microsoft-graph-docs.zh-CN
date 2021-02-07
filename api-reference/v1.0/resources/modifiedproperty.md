---
title: modifiedProperty 资源类型
description: 指示已修改的 Azure AD 资源上的所有属性，包括旧值和新值。
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4e34501f5011310eb7ade73d1c5d938cb58e65cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136036"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="4dd6d-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="4dd6d-103">modifiedProperty resource type</span></span>

<span data-ttu-id="4dd6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dd6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4dd6d-105">指示已修改的 Azure AD 资源上的所有属性，包括旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="4dd6d-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="4dd6d-106">属性</span><span class="sxs-lookup"><span data-stu-id="4dd6d-106">Properties</span></span>

| <span data-ttu-id="4dd6d-107">属性</span><span class="sxs-lookup"><span data-stu-id="4dd6d-107">Property</span></span>     | <span data-ttu-id="4dd6d-108">类型</span><span class="sxs-lookup"><span data-stu-id="4dd6d-108">Type</span></span>   |<span data-ttu-id="4dd6d-109">说明</span><span class="sxs-lookup"><span data-stu-id="4dd6d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dd6d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4dd6d-110">displayName</span></span>|<span data-ttu-id="4dd6d-111">String</span><span class="sxs-lookup"><span data-stu-id="4dd6d-111">String</span></span>|<span data-ttu-id="4dd6d-112">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="4dd6d-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="4dd6d-113">NewValue</span><span class="sxs-lookup"><span data-stu-id="4dd6d-113">newValue</span></span>|<span data-ttu-id="4dd6d-114">String</span><span class="sxs-lookup"><span data-stu-id="4dd6d-114">String</span></span>|<span data-ttu-id="4dd6d-115">指示属性的更新值。</span><span class="sxs-lookup"><span data-stu-id="4dd6d-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="4dd6d-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="4dd6d-116">oldValue</span></span>|<span data-ttu-id="4dd6d-117">String</span><span class="sxs-lookup"><span data-stu-id="4dd6d-117">String</span></span>|<span data-ttu-id="4dd6d-118">指示更新前 (属性) 值。</span><span class="sxs-lookup"><span data-stu-id="4dd6d-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4dd6d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4dd6d-119">JSON representation</span></span>

<span data-ttu-id="4dd6d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dd6d-120">Here is a JSON representation of the resource.</span></span>

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

