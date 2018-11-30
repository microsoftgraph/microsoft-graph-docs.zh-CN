---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041490"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="deedb-102">ChoiceColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="deedb-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="deedb-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="deedb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="deedb-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="deedb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="deedb-105">[columnDefinition](columndefinition.md) 资源上的 **choiceColumn** 指示可从所选列表中选择列的值。</span><span class="sxs-lookup"><span data-stu-id="deedb-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="deedb-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deedb-106">JSON representation</span></span>

<span data-ttu-id="deedb-107">下面是 **choiceColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deedb-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="deedb-108">属性</span><span class="sxs-lookup"><span data-stu-id="deedb-108">Properties</span></span>

| <span data-ttu-id="deedb-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="deedb-109">Property name</span></span>      | <span data-ttu-id="deedb-110">类型</span><span class="sxs-lookup"><span data-stu-id="deedb-110">Type</span></span>               | <span data-ttu-id="deedb-111">说明</span><span class="sxs-lookup"><span data-stu-id="deedb-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="deedb-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="deedb-112">**allowTextEntry**</span></span> | <span data-ttu-id="deedb-113">boolean</span><span class="sxs-lookup"><span data-stu-id="deedb-113">boolean</span></span>            | <span data-ttu-id="deedb-114">如果为 true，则允许配置选择之外的自定义值。</span><span class="sxs-lookup"><span data-stu-id="deedb-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="deedb-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="deedb-115">**choices**</span></span>        | <span data-ttu-id="deedb-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="deedb-116">collection(string)</span></span> | <span data-ttu-id="deedb-117">可用于此列的值列表。</span><span class="sxs-lookup"><span data-stu-id="deedb-117">The list of values available for this column.</span></span>
| <span data-ttu-id="deedb-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="deedb-118">**displayAs**</span></span>      | <span data-ttu-id="deedb-119">string</span><span class="sxs-lookup"><span data-stu-id="deedb-119">string</span></span>             | <span data-ttu-id="deedb-120">选择在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="deedb-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="deedb-121">必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="deedb-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
