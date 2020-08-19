---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6e112d97f67b260c19de9fe0ab104e9dc1ed1d74
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810333"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="e0abf-103">yomiPersonName 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0abf-103">yomiPersonName resource type</span></span>

<span data-ttu-id="e0abf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0abf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0abf-105">为用户提供了一种机制，用于存储有关如何对表示 [contact.personname](personname.md) 资源的语言的非本机扬声器的名称进行发音的信息。</span><span class="sxs-lookup"><span data-stu-id="e0abf-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="e0abf-106">属性</span><span class="sxs-lookup"><span data-stu-id="e0abf-106">Properties</span></span>

| <span data-ttu-id="e0abf-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0abf-107">Property</span></span>     | <span data-ttu-id="e0abf-108">类型</span><span class="sxs-lookup"><span data-stu-id="e0abf-108">Type</span></span>        | <span data-ttu-id="e0abf-109">说明</span><span class="sxs-lookup"><span data-stu-id="e0abf-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="e0abf-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e0abf-110">displayName</span></span>   |<span data-ttu-id="e0abf-111">String</span><span class="sxs-lookup"><span data-stu-id="e0abf-111">String</span></span>       | <span data-ttu-id="e0abf-112">姓和名的发音参考线组合。</span><span class="sxs-lookup"><span data-stu-id="e0abf-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="e0abf-113">前</span><span class="sxs-lookup"><span data-stu-id="e0abf-113">first</span></span>         |<span data-ttu-id="e0abf-114">String</span><span class="sxs-lookup"><span data-stu-id="e0abf-114">String</span></span>       | <span data-ttu-id="e0abf-115">用户名字的发音指南。</span><span class="sxs-lookup"><span data-stu-id="e0abf-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="e0abf-116">末</span><span class="sxs-lookup"><span data-stu-id="e0abf-116">last</span></span>          |<span data-ttu-id="e0abf-117">String</span><span class="sxs-lookup"><span data-stu-id="e0abf-117">String</span></span>       | <span data-ttu-id="e0abf-118">用户姓氏的发音指南。</span><span class="sxs-lookup"><span data-stu-id="e0abf-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="e0abf-119">maiden</span><span class="sxs-lookup"><span data-stu-id="e0abf-119">maiden</span></span>        |<span data-ttu-id="e0abf-120">String</span><span class="sxs-lookup"><span data-stu-id="e0abf-120">String</span></span>       | <span data-ttu-id="e0abf-121">用户的 maiden 名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="e0abf-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="e0abf-122">中间</span><span class="sxs-lookup"><span data-stu-id="e0abf-122">middle</span></span>        |<span data-ttu-id="e0abf-123">String</span><span class="sxs-lookup"><span data-stu-id="e0abf-123">String</span></span>       | <span data-ttu-id="e0abf-124">用户中间名的发音指南。</span><span class="sxs-lookup"><span data-stu-id="e0abf-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="e0abf-125">关系</span><span class="sxs-lookup"><span data-stu-id="e0abf-125">Relationships</span></span>

<span data-ttu-id="e0abf-126">无。</span><span class="sxs-lookup"><span data-stu-id="e0abf-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0abf-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0abf-127">JSON representation</span></span>

<span data-ttu-id="e0abf-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0abf-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yomiPersonName"
}
-->

``` json

{
  "displayName": "String",
  "first": "String",
  "maiden": "String",
  "middle": "String",
  "last": "String"
}
```
