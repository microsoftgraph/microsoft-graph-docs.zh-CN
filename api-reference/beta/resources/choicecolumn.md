---
author: JeremyKelley
description: columnDefinition 资源上的 choiceColumn 指示可从所选列表中选择列的值。
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a5e6efa944756077eb29467be6e75013d4bf28aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021985"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="e62be-103">ChoiceColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="e62be-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="e62be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e62be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e62be-105">[columnDefinition](columndefinition.md) 资源上的 **choiceColumn** 指示可从所选列表中选择列的值。</span><span class="sxs-lookup"><span data-stu-id="e62be-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e62be-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e62be-106">JSON representation</span></span>

<span data-ttu-id="e62be-107">下面是 **choiceColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e62be-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="e62be-108">属性</span><span class="sxs-lookup"><span data-stu-id="e62be-108">Properties</span></span>

| <span data-ttu-id="e62be-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="e62be-109">Property name</span></span>      | <span data-ttu-id="e62be-110">类型</span><span class="sxs-lookup"><span data-stu-id="e62be-110">Type</span></span>               | <span data-ttu-id="e62be-111">说明</span><span class="sxs-lookup"><span data-stu-id="e62be-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="e62be-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="e62be-112">**allowTextEntry**</span></span> | <span data-ttu-id="e62be-113">boolean</span><span class="sxs-lookup"><span data-stu-id="e62be-113">boolean</span></span>            | <span data-ttu-id="e62be-114">如果为 true，则允许配置选择之外的自定义值。</span><span class="sxs-lookup"><span data-stu-id="e62be-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="e62be-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="e62be-115">**choices**</span></span>        | <span data-ttu-id="e62be-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="e62be-116">collection(string)</span></span> | <span data-ttu-id="e62be-117">可用于此列的值列表。</span><span class="sxs-lookup"><span data-stu-id="e62be-117">The list of values available for this column.</span></span>
| <span data-ttu-id="e62be-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="e62be-118">**displayAs**</span></span>      | <span data-ttu-id="e62be-119">string</span><span class="sxs-lookup"><span data-stu-id="e62be-119">string</span></span>             | <span data-ttu-id="e62be-120">选择在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="e62be-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="e62be-121">必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="e62be-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->


