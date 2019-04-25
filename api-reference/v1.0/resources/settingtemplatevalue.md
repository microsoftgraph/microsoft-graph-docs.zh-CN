---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549690"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="b28b1-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="b28b1-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="b28b1-104">表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。</span><span class="sxs-lookup"><span data-stu-id="b28b1-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="b28b1-105">属性</span><span class="sxs-lookup"><span data-stu-id="b28b1-105">Properties</span></span>

| <span data-ttu-id="b28b1-106">属性</span><span class="sxs-lookup"><span data-stu-id="b28b1-106">Property</span></span> | <span data-ttu-id="b28b1-107">类型</span><span class="sxs-lookup"><span data-stu-id="b28b1-107">Type</span></span> | <span data-ttu-id="b28b1-108">说明</span><span class="sxs-lookup"><span data-stu-id="b28b1-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b28b1-109">默认</span><span class="sxs-lookup"><span data-stu-id="b28b1-109">defaultValue</span></span>|<span data-ttu-id="b28b1-110">String</span><span class="sxs-lookup"><span data-stu-id="b28b1-110">String</span></span>| <span data-ttu-id="b28b1-111">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="b28b1-111">Default value for the setting.</span></span> |
|<span data-ttu-id="b28b1-112">description</span><span class="sxs-lookup"><span data-stu-id="b28b1-112">description</span></span>|<span data-ttu-id="b28b1-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b28b1-113">String</span></span>| <span data-ttu-id="b28b1-114">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="b28b1-114">Description of the setting.</span></span> |
|<span data-ttu-id="b28b1-115">name</span><span class="sxs-lookup"><span data-stu-id="b28b1-115">name</span></span>|<span data-ttu-id="b28b1-116">String</span><span class="sxs-lookup"><span data-stu-id="b28b1-116">String</span></span>| <span data-ttu-id="b28b1-117">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="b28b1-117">Name of the setting.</span></span> |
|<span data-ttu-id="b28b1-118">类型</span><span class="sxs-lookup"><span data-stu-id="b28b1-118">type</span></span>|<span data-ttu-id="b28b1-119">String</span><span class="sxs-lookup"><span data-stu-id="b28b1-119">String</span></span>| <span data-ttu-id="b28b1-120">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="b28b1-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="b28b1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b28b1-121">JSON representation</span></span>

<span data-ttu-id="b28b1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b28b1-122">Here is a JSON representation of the resource.</span></span>

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
