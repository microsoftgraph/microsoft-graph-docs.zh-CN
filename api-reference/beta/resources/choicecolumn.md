---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543752"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="6d682-102">ChoiceColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d682-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="6d682-103">[columnDefinition](columndefinition.md) 资源上的 **choiceColumn** 指示可从所选列表中选择列的值。</span><span class="sxs-lookup"><span data-stu-id="6d682-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d682-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d682-104">JSON representation</span></span>

<span data-ttu-id="6d682-105">下面是 **choiceColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d682-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="6d682-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d682-106">Properties</span></span>

| <span data-ttu-id="6d682-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="6d682-107">Property name</span></span>      | <span data-ttu-id="6d682-108">类型</span><span class="sxs-lookup"><span data-stu-id="6d682-108">Type</span></span>               | <span data-ttu-id="6d682-109">说明</span><span class="sxs-lookup"><span data-stu-id="6d682-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="6d682-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="6d682-110">**allowTextEntry**</span></span> | <span data-ttu-id="6d682-111">boolean</span><span class="sxs-lookup"><span data-stu-id="6d682-111">boolean</span></span>            | <span data-ttu-id="6d682-112">如果为 true，则允许配置选择之外的自定义值。</span><span class="sxs-lookup"><span data-stu-id="6d682-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="6d682-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="6d682-113">**choices**</span></span>        | <span data-ttu-id="6d682-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="6d682-114">collection(string)</span></span> | <span data-ttu-id="6d682-115">可用于此列的值列表。</span><span class="sxs-lookup"><span data-stu-id="6d682-115">The list of values available for this column.</span></span>
| <span data-ttu-id="6d682-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="6d682-116">**displayAs**</span></span>      | <span data-ttu-id="6d682-117">string</span><span class="sxs-lookup"><span data-stu-id="6d682-117">string</span></span>             | <span data-ttu-id="6d682-118">选择在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="6d682-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="6d682-119">必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="6d682-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
