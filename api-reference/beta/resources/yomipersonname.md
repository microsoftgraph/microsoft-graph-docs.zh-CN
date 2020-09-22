---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 926479832db04e427e7ca1d73744008db7dc6aaa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079625"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="49360-103">yomiPersonName 资源类型</span><span class="sxs-lookup"><span data-stu-id="49360-103">yomiPersonName resource type</span></span>

<span data-ttu-id="49360-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49360-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49360-105">为用户提供了一种机制，用于存储有关如何对表示 [contact.personname](personname.md) 资源的语言的非本机扬声器的名称进行发音的信息。</span><span class="sxs-lookup"><span data-stu-id="49360-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="49360-106">属性</span><span class="sxs-lookup"><span data-stu-id="49360-106">Properties</span></span>

| <span data-ttu-id="49360-107">属性</span><span class="sxs-lookup"><span data-stu-id="49360-107">Property</span></span>     | <span data-ttu-id="49360-108">类型</span><span class="sxs-lookup"><span data-stu-id="49360-108">Type</span></span>        | <span data-ttu-id="49360-109">说明</span><span class="sxs-lookup"><span data-stu-id="49360-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="49360-110">displayName</span><span class="sxs-lookup"><span data-stu-id="49360-110">displayName</span></span>   |<span data-ttu-id="49360-111">String</span><span class="sxs-lookup"><span data-stu-id="49360-111">String</span></span>       | <span data-ttu-id="49360-112">姓和名的发音参考线组合。</span><span class="sxs-lookup"><span data-stu-id="49360-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="49360-113">前</span><span class="sxs-lookup"><span data-stu-id="49360-113">first</span></span>         |<span data-ttu-id="49360-114">String</span><span class="sxs-lookup"><span data-stu-id="49360-114">String</span></span>       | <span data-ttu-id="49360-115">用户名字的发音指南。</span><span class="sxs-lookup"><span data-stu-id="49360-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="49360-116">末</span><span class="sxs-lookup"><span data-stu-id="49360-116">last</span></span>          |<span data-ttu-id="49360-117">String</span><span class="sxs-lookup"><span data-stu-id="49360-117">String</span></span>       | <span data-ttu-id="49360-118">用户姓氏的发音指南。</span><span class="sxs-lookup"><span data-stu-id="49360-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="49360-119">maiden</span><span class="sxs-lookup"><span data-stu-id="49360-119">maiden</span></span>        |<span data-ttu-id="49360-120">String</span><span class="sxs-lookup"><span data-stu-id="49360-120">String</span></span>       | <span data-ttu-id="49360-121">用户的 maiden 名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="49360-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="49360-122">中间</span><span class="sxs-lookup"><span data-stu-id="49360-122">middle</span></span>        |<span data-ttu-id="49360-123">String</span><span class="sxs-lookup"><span data-stu-id="49360-123">String</span></span>       | <span data-ttu-id="49360-124">用户中间名的发音指南。</span><span class="sxs-lookup"><span data-stu-id="49360-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="49360-125">关系</span><span class="sxs-lookup"><span data-stu-id="49360-125">Relationships</span></span>

<span data-ttu-id="49360-126">无。</span><span class="sxs-lookup"><span data-stu-id="49360-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49360-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49360-127">JSON representation</span></span>

<span data-ttu-id="49360-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49360-128">The following is a JSON representation of the resource.</span></span>
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


