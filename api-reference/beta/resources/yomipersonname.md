---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a598c4b5e999b03aeb7201c6eae3a230d3160a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518971"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="4c46d-103">yomiPersonName 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c46d-103">yomiPersonName resource type</span></span>

<span data-ttu-id="4c46d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4c46d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c46d-105">为用户提供了一种机制，用于存储有关如何对表示[contact.personname](personname.md)资源的语言的非本机扬声器的名称进行发音的信息。</span><span class="sxs-lookup"><span data-stu-id="4c46d-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="4c46d-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c46d-106">Properties</span></span>

| <span data-ttu-id="4c46d-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c46d-107">Property</span></span>     | <span data-ttu-id="4c46d-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c46d-108">Type</span></span>        | <span data-ttu-id="4c46d-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c46d-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="4c46d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4c46d-110">displayName</span></span>   |<span data-ttu-id="4c46d-111">String</span><span class="sxs-lookup"><span data-stu-id="4c46d-111">String</span></span>       | <span data-ttu-id="4c46d-112">姓和名的发音参考线组合。</span><span class="sxs-lookup"><span data-stu-id="4c46d-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="4c46d-113">前</span><span class="sxs-lookup"><span data-stu-id="4c46d-113">first</span></span>         |<span data-ttu-id="4c46d-114">String</span><span class="sxs-lookup"><span data-stu-id="4c46d-114">String</span></span>       | <span data-ttu-id="4c46d-115">用户名字的发音指南。</span><span class="sxs-lookup"><span data-stu-id="4c46d-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="4c46d-116">末</span><span class="sxs-lookup"><span data-stu-id="4c46d-116">last</span></span>          |<span data-ttu-id="4c46d-117">String</span><span class="sxs-lookup"><span data-stu-id="4c46d-117">String</span></span>       | <span data-ttu-id="4c46d-118">用户姓氏的发音指南。</span><span class="sxs-lookup"><span data-stu-id="4c46d-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="4c46d-119">maiden</span><span class="sxs-lookup"><span data-stu-id="4c46d-119">maiden</span></span>        |<span data-ttu-id="4c46d-120">String</span><span class="sxs-lookup"><span data-stu-id="4c46d-120">String</span></span>       | <span data-ttu-id="4c46d-121">用户的 maiden 名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="4c46d-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="4c46d-122">中间</span><span class="sxs-lookup"><span data-stu-id="4c46d-122">middle</span></span>        |<span data-ttu-id="4c46d-123">String</span><span class="sxs-lookup"><span data-stu-id="4c46d-123">String</span></span>       | <span data-ttu-id="4c46d-124">用户中间名的发音指南。</span><span class="sxs-lookup"><span data-stu-id="4c46d-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="4c46d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c46d-125">JSON representation</span></span>

<span data-ttu-id="4c46d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c46d-126">The following is a JSON representation of the resource.</span></span>

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
