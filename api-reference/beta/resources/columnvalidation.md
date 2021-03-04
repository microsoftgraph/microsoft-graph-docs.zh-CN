---
author: swapnil1993
title: columnValidation 资源类型
description: 包含用于验证列值的数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c1b20b239b894aa0da63222bb69a8d720e5ab50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446626"
---
# <a name="columnvalidation-resource-type"></a><span data-ttu-id="ce2fd-103">columnValidation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce2fd-103">columnValidation resource type</span></span>

<span data-ttu-id="ce2fd-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="ce2fd-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>
<span data-ttu-id="ce2fd-105">包含用于验证列的元数据。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-105">Contains metadata for validating the column.</span></span>


## <a name="properties"></a><span data-ttu-id="ce2fd-106">属性</span><span class="sxs-lookup"><span data-stu-id="ce2fd-106">Properties</span></span>

| <span data-ttu-id="ce2fd-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="ce2fd-107">Property name</span></span>  | <span data-ttu-id="ce2fd-108">类型</span><span class="sxs-lookup"><span data-stu-id="ce2fd-108">Type</span></span>    | <span data-ttu-id="ce2fd-109">说明</span><span class="sxs-lookup"><span data-stu-id="ce2fd-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="ce2fd-110">**formula**</span><span class="sxs-lookup"><span data-stu-id="ce2fd-110">**formula**</span></span>    | <span data-ttu-id="ce2fd-111">string</span><span class="sxs-lookup"><span data-stu-id="ce2fd-111">string</span></span>  | <span data-ttu-id="ce2fd-112">用于验证列值的公式。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-112">The formula to validate column value.</span></span> <span data-ttu-id="ce2fd-113">有关示例，请参阅 [列表中常用公式的示例](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)</span><span class="sxs-lookup"><span data-stu-id="ce2fd-113">For examples, see [Examples of common formulas in lists](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)</span></span> 
| <span data-ttu-id="ce2fd-114">**说明**</span><span class="sxs-lookup"><span data-stu-id="ce2fd-114">**descriptions**</span></span>    | <span data-ttu-id="ce2fd-115">集合 (microsoft.graph.displayNameLocalization) </span><span class="sxs-lookup"><span data-stu-id="ce2fd-115">Collection(microsoft.graph.displayNameLocalization)</span></span>  | <span data-ttu-id="ce2fd-116">解释此列的值被视为有效的所需内容的本地化邮件。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-116">Localized messages that explain what is needed for this column's value to be considered valid.</span></span> <span data-ttu-id="ce2fd-117">验证失败时，将提示用户显示此消息。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-117">User will be prompted with this message if validation fails.</span></span> 
| <span data-ttu-id="ce2fd-118">**defaultLanguage**</span><span class="sxs-lookup"><span data-stu-id="ce2fd-118">**defaultLanguage**</span></span>    | <span data-ttu-id="ce2fd-119">string</span><span class="sxs-lookup"><span data-stu-id="ce2fd-119">string</span></span>  | <span data-ttu-id="ce2fd-120">说明的默认 BCP 47 语言标记。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-120">Default BCP 47 language tag for the description.</span></span>

<span data-ttu-id="ce2fd-121">SharePoint 公式使用一种类似于 Excel 公式的语法。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="ce2fd-122">有关详细信息 [，请参阅 SharePoint 列表中][SPFormulas] 常见公式的示例。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce2fd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce2fd-123">JSON representation</span></span>

<span data-ttu-id="ce2fd-124">以下是 **columnValidation** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce2fd-124">The following is a JSON representation of a **columnValidation** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
