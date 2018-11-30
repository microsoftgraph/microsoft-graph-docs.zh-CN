---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011703"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="d7152-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7152-103">settingValue resource type</span></span>

<span data-ttu-id="d7152-104">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="d7152-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="d7152-105">属性</span><span class="sxs-lookup"><span data-stu-id="d7152-105">Properties</span></span>

| <span data-ttu-id="d7152-106">属性</span><span class="sxs-lookup"><span data-stu-id="d7152-106">Property</span></span> | <span data-ttu-id="d7152-107">类型</span><span class="sxs-lookup"><span data-stu-id="d7152-107">Type</span></span> | <span data-ttu-id="d7152-108">说明</span><span class="sxs-lookup"><span data-stu-id="d7152-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d7152-109">name</span><span class="sxs-lookup"><span data-stu-id="d7152-109">name</span></span>|<span data-ttu-id="d7152-110">字符串</span><span class="sxs-lookup"><span data-stu-id="d7152-110">String</span></span>| <span data-ttu-id="d7152-111">设置的名称（由 [groupSettingTemplate](groupsettingtemplate.md) 定义）。</span><span class="sxs-lookup"><span data-stu-id="d7152-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="d7152-112">value</span><span class="sxs-lookup"><span data-stu-id="d7152-112">value</span></span>|<span data-ttu-id="d7152-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d7152-113">String</span></span>| <span data-ttu-id="d7152-114">设置的值。</span><span class="sxs-lookup"><span data-stu-id="d7152-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="d7152-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7152-115">JSON representation</span></span>

<span data-ttu-id="d7152-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7152-116">Here is a JSON representation of the resource.</span></span>

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