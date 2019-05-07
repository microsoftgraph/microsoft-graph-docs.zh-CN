---
title: modifiedProperty 资源类型
description: 指示 Azure AD 资源中已修改的所有属性, 包括旧值和新值。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: d87d0170dc811db074026e60efc63df928c65ada
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629276"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="05c07-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="05c07-103">modifiedProperty resource type</span></span>

<span data-ttu-id="05c07-104">指示 Azure AD 资源中已修改的所有属性, 包括旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="05c07-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="05c07-105">属性</span><span class="sxs-lookup"><span data-stu-id="05c07-105">Properties</span></span>

| <span data-ttu-id="05c07-106">属性</span><span class="sxs-lookup"><span data-stu-id="05c07-106">Property</span></span>     | <span data-ttu-id="05c07-107">类型</span><span class="sxs-lookup"><span data-stu-id="05c07-107">Type</span></span>   |<span data-ttu-id="05c07-108">说明</span><span class="sxs-lookup"><span data-stu-id="05c07-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05c07-109">displayName</span><span class="sxs-lookup"><span data-stu-id="05c07-109">displayName</span></span>|<span data-ttu-id="05c07-110">String</span><span class="sxs-lookup"><span data-stu-id="05c07-110">String</span></span>|<span data-ttu-id="05c07-111">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="05c07-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="05c07-112">NewValue</span><span class="sxs-lookup"><span data-stu-id="05c07-112">newValue</span></span>|<span data-ttu-id="05c07-113">String</span><span class="sxs-lookup"><span data-stu-id="05c07-113">String</span></span>|<span data-ttu-id="05c07-114">指示值的更新值。</span><span class="sxs-lookup"><span data-stu-id="05c07-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="05c07-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="05c07-115">oldValue</span></span>|<span data-ttu-id="05c07-116">字符串</span><span class="sxs-lookup"><span data-stu-id="05c07-116">String</span></span>|<span data-ttu-id="05c07-117">指示属性的前一个值 (在更新之前)。</span><span class="sxs-lookup"><span data-stu-id="05c07-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05c07-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05c07-118">JSON representation</span></span>

<span data-ttu-id="05c07-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05c07-119">Here is a JSON representation of the resource.</span></span>

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
