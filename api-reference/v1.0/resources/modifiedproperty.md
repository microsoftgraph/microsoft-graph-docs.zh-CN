---
title: modifiedProperty 资源类型
description: 指示 Azure AD 资源中已修改的所有属性，包括旧值和新值。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 13d377f05650f50f9f87f618ca1c9c07d1da70ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534221"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="fe7bc-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe7bc-103">modifiedProperty resource type</span></span>

<span data-ttu-id="fe7bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe7bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe7bc-105">指示 Azure AD 资源中已修改的所有属性，包括旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="fe7bc-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="fe7bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="fe7bc-106">Properties</span></span>

| <span data-ttu-id="fe7bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="fe7bc-107">Property</span></span>     | <span data-ttu-id="fe7bc-108">类型</span><span class="sxs-lookup"><span data-stu-id="fe7bc-108">Type</span></span>   |<span data-ttu-id="fe7bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="fe7bc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe7bc-110">displayName</span><span class="sxs-lookup"><span data-stu-id="fe7bc-110">displayName</span></span>|<span data-ttu-id="fe7bc-111">String</span><span class="sxs-lookup"><span data-stu-id="fe7bc-111">String</span></span>|<span data-ttu-id="fe7bc-112">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="fe7bc-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="fe7bc-113">NewValue</span><span class="sxs-lookup"><span data-stu-id="fe7bc-113">newValue</span></span>|<span data-ttu-id="fe7bc-114">String</span><span class="sxs-lookup"><span data-stu-id="fe7bc-114">String</span></span>|<span data-ttu-id="fe7bc-115">指示值的更新值。</span><span class="sxs-lookup"><span data-stu-id="fe7bc-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="fe7bc-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="fe7bc-116">oldValue</span></span>|<span data-ttu-id="fe7bc-117">字符串</span><span class="sxs-lookup"><span data-stu-id="fe7bc-117">String</span></span>|<span data-ttu-id="fe7bc-118">指示属性的前一个值（在更新之前）。</span><span class="sxs-lookup"><span data-stu-id="fe7bc-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe7bc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe7bc-119">JSON representation</span></span>

<span data-ttu-id="fe7bc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe7bc-120">Here is a JSON representation of the resource.</span></span>

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
