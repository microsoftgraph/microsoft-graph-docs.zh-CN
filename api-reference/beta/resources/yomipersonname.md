---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8117dd71947fea41508ccbe7d50d49a4f78b335d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939766"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="44776-103">yomiPersonName 资源类型</span><span class="sxs-lookup"><span data-stu-id="44776-103">yomiPersonName resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44776-104">为用户提供了一种机制，用于存储有关如何对表示[contact.personname](personname.md)资源的语言的非本机扬声器的名称进行发音的信息。</span><span class="sxs-lookup"><span data-stu-id="44776-104">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="44776-105">属性</span><span class="sxs-lookup"><span data-stu-id="44776-105">Properties</span></span>

| <span data-ttu-id="44776-106">属性</span><span class="sxs-lookup"><span data-stu-id="44776-106">Property</span></span>     | <span data-ttu-id="44776-107">类型</span><span class="sxs-lookup"><span data-stu-id="44776-107">Type</span></span>        | <span data-ttu-id="44776-108">说明</span><span class="sxs-lookup"><span data-stu-id="44776-108">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="44776-109">displayName</span><span class="sxs-lookup"><span data-stu-id="44776-109">displayName</span></span>   |<span data-ttu-id="44776-110">String</span><span class="sxs-lookup"><span data-stu-id="44776-110">String</span></span>       | <span data-ttu-id="44776-111">姓和名的发音参考线组合。</span><span class="sxs-lookup"><span data-stu-id="44776-111">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="44776-112">前</span><span class="sxs-lookup"><span data-stu-id="44776-112">first</span></span>         |<span data-ttu-id="44776-113">字符串</span><span class="sxs-lookup"><span data-stu-id="44776-113">String</span></span>       | <span data-ttu-id="44776-114">用户名字的发音指南。</span><span class="sxs-lookup"><span data-stu-id="44776-114">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="44776-115">末</span><span class="sxs-lookup"><span data-stu-id="44776-115">last</span></span>          |<span data-ttu-id="44776-116">字符串</span><span class="sxs-lookup"><span data-stu-id="44776-116">String</span></span>       | <span data-ttu-id="44776-117">用户姓氏的发音指南。</span><span class="sxs-lookup"><span data-stu-id="44776-117">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="44776-118">maiden</span><span class="sxs-lookup"><span data-stu-id="44776-118">maiden</span></span>        |<span data-ttu-id="44776-119">字符串</span><span class="sxs-lookup"><span data-stu-id="44776-119">String</span></span>       | <span data-ttu-id="44776-120">用户的 maiden 名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="44776-120">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="44776-121">中间</span><span class="sxs-lookup"><span data-stu-id="44776-121">middle</span></span>        |<span data-ttu-id="44776-122">字符串</span><span class="sxs-lookup"><span data-stu-id="44776-122">String</span></span>       | <span data-ttu-id="44776-123">用户中间名的发音指南。</span><span class="sxs-lookup"><span data-stu-id="44776-123">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="44776-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44776-124">JSON representation</span></span>

<span data-ttu-id="44776-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44776-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
