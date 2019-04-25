---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: f38fc2a29a5fdee77456a5ceee7c7689cfe3f412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543220"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="2be99-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="2be99-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="2be99-103">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="2be99-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2be99-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2be99-104">JSON representation</span></span>

<span data-ttu-id="2be99-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2be99-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="2be99-106">属性</span><span class="sxs-lookup"><span data-stu-id="2be99-106">Properties</span></span>

| <span data-ttu-id="2be99-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="2be99-107">Property name</span></span> | <span data-ttu-id="2be99-108">类型</span><span class="sxs-lookup"><span data-stu-id="2be99-108">Type</span></span>   | <span data-ttu-id="2be99-109">说明</span><span class="sxs-lookup"><span data-stu-id="2be99-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2be99-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="2be99-110">**locale**</span></span>    | <span data-ttu-id="2be99-111">string</span><span class="sxs-lookup"><span data-stu-id="2be99-111">string</span></span> | <span data-ttu-id="2be99-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="2be99-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
