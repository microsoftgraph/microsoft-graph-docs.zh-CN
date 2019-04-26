---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549683"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="8f3f6-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f3f6-103">settingValue resource type</span></span>

<span data-ttu-id="8f3f6-104">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="8f3f6-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="8f3f6-105">属性</span><span class="sxs-lookup"><span data-stu-id="8f3f6-105">Properties</span></span>

| <span data-ttu-id="8f3f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="8f3f6-106">Property</span></span> | <span data-ttu-id="8f3f6-107">类型</span><span class="sxs-lookup"><span data-stu-id="8f3f6-107">Type</span></span> | <span data-ttu-id="8f3f6-108">说明</span><span class="sxs-lookup"><span data-stu-id="8f3f6-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8f3f6-109">name</span><span class="sxs-lookup"><span data-stu-id="8f3f6-109">name</span></span>|<span data-ttu-id="8f3f6-110">String</span><span class="sxs-lookup"><span data-stu-id="8f3f6-110">String</span></span>| <span data-ttu-id="8f3f6-111">设置的名称 (由[groupSettingTemplate](groupsettingtemplate.md)定义)。</span><span class="sxs-lookup"><span data-stu-id="8f3f6-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="8f3f6-112">value</span><span class="sxs-lookup"><span data-stu-id="8f3f6-112">value</span></span>|<span data-ttu-id="8f3f6-113">String</span><span class="sxs-lookup"><span data-stu-id="8f3f6-113">String</span></span>| <span data-ttu-id="8f3f6-114">设置的值。</span><span class="sxs-lookup"><span data-stu-id="8f3f6-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="8f3f6-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f3f6-115">JSON representation</span></span>

<span data-ttu-id="8f3f6-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f3f6-116">Here is a JSON representation of the resource.</span></span>

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
