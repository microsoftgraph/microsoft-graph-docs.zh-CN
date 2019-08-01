---
title: modifiedProperty 资源类型
description: 指示 Azure AD 资源中已修改的所有属性, 包括旧值和新值。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 0c5375ea3e188d6023e3588531e07877f6de38ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036097"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="0b4dd-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b4dd-103">modifiedProperty resource type</span></span>

<span data-ttu-id="0b4dd-104">指示 Azure AD 资源中已修改的所有属性, 包括旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="0b4dd-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="0b4dd-105">属性</span><span class="sxs-lookup"><span data-stu-id="0b4dd-105">Properties</span></span>

| <span data-ttu-id="0b4dd-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b4dd-106">Property</span></span>     | <span data-ttu-id="0b4dd-107">类型</span><span class="sxs-lookup"><span data-stu-id="0b4dd-107">Type</span></span>   |<span data-ttu-id="0b4dd-108">说明</span><span class="sxs-lookup"><span data-stu-id="0b4dd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b4dd-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0b4dd-109">displayName</span></span>|<span data-ttu-id="0b4dd-110">String</span><span class="sxs-lookup"><span data-stu-id="0b4dd-110">String</span></span>|<span data-ttu-id="0b4dd-111">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="0b4dd-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="0b4dd-112">NewValue</span><span class="sxs-lookup"><span data-stu-id="0b4dd-112">newValue</span></span>|<span data-ttu-id="0b4dd-113">String</span><span class="sxs-lookup"><span data-stu-id="0b4dd-113">String</span></span>|<span data-ttu-id="0b4dd-114">指示值的更新值。</span><span class="sxs-lookup"><span data-stu-id="0b4dd-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="0b4dd-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="0b4dd-115">oldValue</span></span>|<span data-ttu-id="0b4dd-116">String</span><span class="sxs-lookup"><span data-stu-id="0b4dd-116">String</span></span>|<span data-ttu-id="0b4dd-117">指示属性的前一个值 (在更新之前)。</span><span class="sxs-lookup"><span data-stu-id="0b4dd-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b4dd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b4dd-118">JSON representation</span></span>

<span data-ttu-id="0b4dd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b4dd-119">Here is a JSON representation of the resource.</span></span>

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
