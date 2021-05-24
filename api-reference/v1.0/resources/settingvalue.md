---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 171b08d4542af6900dcb6549527e956c4395c947
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547041"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="d5f30-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5f30-103">settingValue resource type</span></span>

<span data-ttu-id="d5f30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5f30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5f30-105">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="d5f30-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="d5f30-106">属性</span><span class="sxs-lookup"><span data-stu-id="d5f30-106">Properties</span></span>

| <span data-ttu-id="d5f30-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5f30-107">Property</span></span> | <span data-ttu-id="d5f30-108">类型</span><span class="sxs-lookup"><span data-stu-id="d5f30-108">Type</span></span> | <span data-ttu-id="d5f30-109">描述</span><span class="sxs-lookup"><span data-stu-id="d5f30-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d5f30-110">name</span><span class="sxs-lookup"><span data-stu-id="d5f30-110">name</span></span>|<span data-ttu-id="d5f30-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d5f30-111">String</span></span>| <span data-ttu-id="d5f30-112">[groupSettingTemplate](groupsettingtemplate.md) (定义的设置) 。</span><span class="sxs-lookup"><span data-stu-id="d5f30-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="d5f30-113">value</span><span class="sxs-lookup"><span data-stu-id="d5f30-113">value</span></span>|<span data-ttu-id="d5f30-114">String</span><span class="sxs-lookup"><span data-stu-id="d5f30-114">String</span></span>| <span data-ttu-id="d5f30-115">设置的值。</span><span class="sxs-lookup"><span data-stu-id="d5f30-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="d5f30-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5f30-116">JSON representation</span></span>

<span data-ttu-id="d5f30-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5f30-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

