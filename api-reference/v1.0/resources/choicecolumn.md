---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="2a0a3-102">ChoiceColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a0a3-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="2a0a3-103">[columnDefinition](columnDefinition.md) 资源上的 **choiceColumn** 指示可从选项列表中选择的列的值。</span><span class="sxs-lookup"><span data-stu-id="2a0a3-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a0a3-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a0a3-104">JSON representation</span></span>

<span data-ttu-id="2a0a3-105">下面是 **choiceColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a0a3-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="2a0a3-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a0a3-106">Properties</span></span>

| <span data-ttu-id="2a0a3-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="2a0a3-107">Property name</span></span>      | <span data-ttu-id="2a0a3-108">类型</span><span class="sxs-lookup"><span data-stu-id="2a0a3-108">Type</span></span>               | <span data-ttu-id="2a0a3-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a0a3-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="2a0a3-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="2a0a3-110">**allowTextEntry**</span></span> | <span data-ttu-id="2a0a3-111">boolean</span><span class="sxs-lookup"><span data-stu-id="2a0a3-111">boolean</span></span>            | <span data-ttu-id="2a0a3-112">如果为 true，则允许配置选择之外的自定义值。</span><span class="sxs-lookup"><span data-stu-id="2a0a3-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="2a0a3-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="2a0a3-113">**Choices**</span></span>        | <span data-ttu-id="2a0a3-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="2a0a3-114">Collection(String)</span></span> | <span data-ttu-id="2a0a3-115">可用于此列的值的列表。</span><span class="sxs-lookup"><span data-stu-id="2a0a3-115">The list of values available for this column.</span></span>
| <span data-ttu-id="2a0a3-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="2a0a3-116">**displayAs**</span></span>      | <span data-ttu-id="2a0a3-117">string</span><span class="sxs-lookup"><span data-stu-id="2a0a3-117">string</span></span>             | <span data-ttu-id="2a0a3-118">选择在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="2a0a3-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="2a0a3-119">必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="2a0a3-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
