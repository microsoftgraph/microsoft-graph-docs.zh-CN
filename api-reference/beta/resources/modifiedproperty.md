---
title: modifiedProperty 资源类型
description: 指示已更改的 Azure AD 中与旧值和新值的任何资源所有修改的属性
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844450"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="5b310-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b310-103">modifiedProperty resource type</span></span>
<span data-ttu-id="5b310-104">指示已更改的 Azure AD 中与旧值和新值的任何资源所有修改的属性</span><span class="sxs-lookup"><span data-stu-id="5b310-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="5b310-105">属性</span><span class="sxs-lookup"><span data-stu-id="5b310-105">Properties</span></span>
| <span data-ttu-id="5b310-106">属性</span><span class="sxs-lookup"><span data-stu-id="5b310-106">Property</span></span>     | <span data-ttu-id="5b310-107">类型</span><span class="sxs-lookup"><span data-stu-id="5b310-107">Type</span></span>   |<span data-ttu-id="5b310-108">说明</span><span class="sxs-lookup"><span data-stu-id="5b310-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b310-109">displayName</span><span class="sxs-lookup"><span data-stu-id="5b310-109">displayName</span></span>|<span data-ttu-id="5b310-110">字符串</span><span class="sxs-lookup"><span data-stu-id="5b310-110">String</span></span>|<span data-ttu-id="5b310-111">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="5b310-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="5b310-112">NewValue</span><span class="sxs-lookup"><span data-stu-id="5b310-112">newValue</span></span>|<span data-ttu-id="5b310-113">String</span><span class="sxs-lookup"><span data-stu-id="5b310-113">String</span></span>|<span data-ttu-id="5b310-114">指示更新属性的值。</span><span class="sxs-lookup"><span data-stu-id="5b310-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="5b310-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="5b310-115">oldValue</span></span>|<span data-ttu-id="5b310-116">String</span><span class="sxs-lookup"><span data-stu-id="5b310-116">String</span></span>|<span data-ttu-id="5b310-117">指示前的数值 （更新） 的属性。</span><span class="sxs-lookup"><span data-stu-id="5b310-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b310-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b310-118">JSON representation</span></span>

<span data-ttu-id="5b310-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b310-119">Here is a JSON representation of the resource.</span></span>

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
