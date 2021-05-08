---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41a878f58736f608cf9cc9f0c45867bf48669b1a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231834"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="0603d-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="0603d-105">educationTerm resource type</span></span>

<span data-ttu-id="0603d-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0603d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0603d-107">一个学期。</span><span class="sxs-lookup"><span data-stu-id="0603d-107">A term.</span></span> <span data-ttu-id="0603d-108">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="0603d-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="0603d-109">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="0603d-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0603d-110">属性</span><span class="sxs-lookup"><span data-stu-id="0603d-110">Properties</span></span>

| <span data-ttu-id="0603d-111">属性</span><span class="sxs-lookup"><span data-stu-id="0603d-111">Property</span></span>    | <span data-ttu-id="0603d-112">类型</span><span class="sxs-lookup"><span data-stu-id="0603d-112">Type</span></span>   | <span data-ttu-id="0603d-113">说明</span><span class="sxs-lookup"><span data-stu-id="0603d-113">Description</span></span>                       |
| :---------- | :----- | :-------------------------------- |
| <span data-ttu-id="0603d-114">displayName</span><span class="sxs-lookup"><span data-stu-id="0603d-114">displayName</span></span> | <span data-ttu-id="0603d-115">String</span><span class="sxs-lookup"><span data-stu-id="0603d-115">String</span></span> | <span data-ttu-id="0603d-116">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0603d-116">Display name of the term.</span></span>         |
| <span data-ttu-id="0603d-117">externalId</span><span class="sxs-lookup"><span data-stu-id="0603d-117">externalId</span></span>  | <span data-ttu-id="0603d-118">String</span><span class="sxs-lookup"><span data-stu-id="0603d-118">String</span></span> | <span data-ttu-id="0603d-119">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="0603d-119">ID of term in the syncing system.</span></span> |
| <span data-ttu-id="0603d-120">startDate</span><span class="sxs-lookup"><span data-stu-id="0603d-120">startDate</span></span>   | <span data-ttu-id="0603d-121">Date</span><span class="sxs-lookup"><span data-stu-id="0603d-121">Date</span></span>   | <span data-ttu-id="0603d-122">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="0603d-122">Start of the term.</span></span>                |
| <span data-ttu-id="0603d-123">endDate</span><span class="sxs-lookup"><span data-stu-id="0603d-123">endDate</span></span>     | <span data-ttu-id="0603d-124">Date</span><span class="sxs-lookup"><span data-stu-id="0603d-124">Date</span></span>   | <span data-ttu-id="0603d-125">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="0603d-125">End of the term.</span></span>                  |

## <a name="relationships"></a><span data-ttu-id="0603d-126">关系</span><span class="sxs-lookup"><span data-stu-id="0603d-126">Relationships</span></span>

<span data-ttu-id="0603d-127">无。</span><span class="sxs-lookup"><span data-stu-id="0603d-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0603d-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0603d-128">JSON representation</span></span>

<span data-ttu-id="0603d-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0603d-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTerm"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTerm",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date",
  "displayName": "String"
}
```
