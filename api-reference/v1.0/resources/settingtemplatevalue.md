---
title: settingTemplateValue 资源类型
description: 如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。
ms.openlocfilehash: 00e424e36338855d8ef603d06c7a9ee52a99c621
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011110"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="ec62d-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec62d-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="ec62d-104">如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="ec62d-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="ec62d-105">属性</span><span class="sxs-lookup"><span data-stu-id="ec62d-105">Properties</span></span>

| <span data-ttu-id="ec62d-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec62d-106">Property</span></span> | <span data-ttu-id="ec62d-107">类型</span><span class="sxs-lookup"><span data-stu-id="ec62d-107">Type</span></span> | <span data-ttu-id="ec62d-108">说明</span><span class="sxs-lookup"><span data-stu-id="ec62d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ec62d-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="ec62d-109">defaultValue</span></span>|<span data-ttu-id="ec62d-110">字符串</span><span class="sxs-lookup"><span data-stu-id="ec62d-110">String</span></span>| <span data-ttu-id="ec62d-111">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="ec62d-111">Default value for the setting.</span></span> |
|<span data-ttu-id="ec62d-112">description</span><span class="sxs-lookup"><span data-stu-id="ec62d-112">description</span></span>|<span data-ttu-id="ec62d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ec62d-113">String</span></span>| <span data-ttu-id="ec62d-114">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="ec62d-114">Description of the setting.</span></span> |
|<span data-ttu-id="ec62d-115">name</span><span class="sxs-lookup"><span data-stu-id="ec62d-115">name</span></span>|<span data-ttu-id="ec62d-116">字符串</span><span class="sxs-lookup"><span data-stu-id="ec62d-116">String</span></span>| <span data-ttu-id="ec62d-117">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="ec62d-117">Name of the setting.</span></span> |
|<span data-ttu-id="ec62d-118">type</span><span class="sxs-lookup"><span data-stu-id="ec62d-118">type</span></span>|<span data-ttu-id="ec62d-119">字符串</span><span class="sxs-lookup"><span data-stu-id="ec62d-119">String</span></span>| <span data-ttu-id="ec62d-120">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="ec62d-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="ec62d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec62d-121">JSON representation</span></span>

<span data-ttu-id="ec62d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec62d-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->