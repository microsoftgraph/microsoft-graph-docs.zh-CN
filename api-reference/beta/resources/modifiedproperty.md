---
title: modifiedProperty 资源类型
description: 指示 Azure AD 中所有已更改的资源的旧值和新值的所有已修改属性
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506234"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="6b10c-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b10c-103">modifiedProperty resource type</span></span>
<span data-ttu-id="6b10c-104">指示 Azure AD 中所有已更改的资源的旧值和新值的所有已修改属性</span><span class="sxs-lookup"><span data-stu-id="6b10c-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="6b10c-105">属性</span><span class="sxs-lookup"><span data-stu-id="6b10c-105">Properties</span></span>
| <span data-ttu-id="6b10c-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b10c-106">Property</span></span>     | <span data-ttu-id="6b10c-107">类型</span><span class="sxs-lookup"><span data-stu-id="6b10c-107">Type</span></span>   |<span data-ttu-id="6b10c-108">说明</span><span class="sxs-lookup"><span data-stu-id="6b10c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b10c-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6b10c-109">displayName</span></span>|<span data-ttu-id="6b10c-110">String</span><span class="sxs-lookup"><span data-stu-id="6b10c-110">String</span></span>|<span data-ttu-id="6b10c-111">指示已更改的目标属性的属性名称。</span><span class="sxs-lookup"><span data-stu-id="6b10c-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="6b10c-112">NewValue</span><span class="sxs-lookup"><span data-stu-id="6b10c-112">newValue</span></span>|<span data-ttu-id="6b10c-113">String</span><span class="sxs-lookup"><span data-stu-id="6b10c-113">String</span></span>|<span data-ttu-id="6b10c-114">指示值的更新值。</span><span class="sxs-lookup"><span data-stu-id="6b10c-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="6b10c-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="6b10c-115">oldValue</span></span>|<span data-ttu-id="6b10c-116">字符串</span><span class="sxs-lookup"><span data-stu-id="6b10c-116">String</span></span>|<span data-ttu-id="6b10c-117">指示属性的前一个值 (在更新之前)。</span><span class="sxs-lookup"><span data-stu-id="6b10c-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b10c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b10c-118">JSON representation</span></span>

<span data-ttu-id="6b10c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b10c-119">Here is a JSON representation of the resource.</span></span>

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
