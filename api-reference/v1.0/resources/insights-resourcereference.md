---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa00eb06ac239b4f93a200e72ecbe88c99d6189c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532869"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="70645-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="70645-103">resourceReference resource type</span></span>

<span data-ttu-id="70645-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70645-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70645-105">包含[officeGraphInsights](officegraphinsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="70645-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="70645-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70645-106">JSON representation</span></span>

<span data-ttu-id="70645-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70645-107">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="70645-108">属性</span><span class="sxs-lookup"><span data-stu-id="70645-108">Properties</span></span>

| <span data-ttu-id="70645-109">属性</span><span class="sxs-lookup"><span data-stu-id="70645-109">Property</span></span>      | <span data-ttu-id="70645-110">类型</span><span class="sxs-lookup"><span data-stu-id="70645-110">Type</span></span>      | <span data-ttu-id="70645-111">说明</span><span class="sxs-lookup"><span data-stu-id="70645-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="70645-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="70645-112">webUrl</span></span>        | <span data-ttu-id="70645-113">String</span><span class="sxs-lookup"><span data-stu-id="70645-113">String</span></span>    | <span data-ttu-id="70645-114">指向引用项的 URL。</span><span class="sxs-lookup"><span data-stu-id="70645-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="70645-115">id</span><span class="sxs-lookup"><span data-stu-id="70645-115">id</span></span>            | <span data-ttu-id="70645-116">String</span><span class="sxs-lookup"><span data-stu-id="70645-116">String</span></span>    | <span data-ttu-id="70645-117">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="70645-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="70645-118">type</span><span class="sxs-lookup"><span data-stu-id="70645-118">type</span></span>          | <span data-ttu-id="70645-119">字符串</span><span class="sxs-lookup"><span data-stu-id="70645-119">String</span></span>    | <span data-ttu-id="70645-120">一个可用于对项目进行分类的字符串值，例如 "driveItem"</span><span class="sxs-lookup"><span data-stu-id="70645-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
