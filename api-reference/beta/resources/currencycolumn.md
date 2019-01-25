---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: c89d709c93eeee0003d193d620166f8abffd9d41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524497"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="ac93a-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac93a-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac93a-103">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="ac93a-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac93a-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac93a-104">JSON representation</span></span>

<span data-ttu-id="ac93a-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac93a-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="ac93a-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac93a-106">Properties</span></span>

| <span data-ttu-id="ac93a-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="ac93a-107">Property name</span></span> | <span data-ttu-id="ac93a-108">类型</span><span class="sxs-lookup"><span data-stu-id="ac93a-108">Type</span></span>   | <span data-ttu-id="ac93a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac93a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ac93a-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="ac93a-110">**locale**</span></span>    | <span data-ttu-id="ac93a-111">string</span><span class="sxs-lookup"><span data-stu-id="ac93a-111">string</span></span> | <span data-ttu-id="ac93a-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="ac93a-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/currencycolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
