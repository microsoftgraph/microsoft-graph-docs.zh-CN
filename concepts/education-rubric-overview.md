---
title: 教育版评分标准概述
description: 评分标准是一种被广泛采用的有效作业评分方式，Microsoft Graph 中的教育版 API 支持它们。
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: 56b9bcdf32036361fb92fe372952c94d09d8dc57
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173081"
---
# <a name="education-rubric-overview"></a><span data-ttu-id="45342-103">教育版评分标准概述</span><span class="sxs-lookup"><span data-stu-id="45342-103">Education rubric overview</span></span>

<span data-ttu-id="45342-104">评分标准是一种被广泛采用的有效作业评分方式，Microsoft Graph 中的教育版 API 支持它们。</span><span class="sxs-lookup"><span data-stu-id="45342-104">Rubrics are an effective and widely-used way of grading assignments, and the education API in Microsoft Graph supports them.</span></span>

<span data-ttu-id="45342-105">评分标准是一个*质量*、*级别*和*条件*矩阵，如下所示：</span><span class="sxs-lookup"><span data-stu-id="45342-105">A grading rubric is a matrix of *qualities*, *levels*, and *criteria*, as follows:</span></span>

| | <span data-ttu-id="45342-106">级别</span><span class="sxs-lookup"><span data-stu-id="45342-106">Level</span></span> | <span data-ttu-id="45342-107">级别</span><span class="sxs-lookup"><span data-stu-id="45342-107">Level</span></span> |
|:--|:--|:--|
| <span data-ttu-id="45342-108">质量</span><span class="sxs-lookup"><span data-stu-id="45342-108">Quality</span></span> | <span data-ttu-id="45342-109">条件</span><span class="sxs-lookup"><span data-stu-id="45342-109">Criterion</span></span> | <span data-ttu-id="45342-110">条件</span><span class="sxs-lookup"><span data-stu-id="45342-110">Criterion</span></span> |
| <span data-ttu-id="45342-111">质量</span><span class="sxs-lookup"><span data-stu-id="45342-111">Quality</span></span> | <span data-ttu-id="45342-112">条件</span><span class="sxs-lookup"><span data-stu-id="45342-112">Criterion</span></span> | <span data-ttu-id="45342-113">条件</span><span class="sxs-lookup"><span data-stu-id="45342-113">Criterion</span></span> |

<span data-ttu-id="45342-114">评分标准示例如下：</span><span class="sxs-lookup"><span data-stu-id="45342-114">An example of a grading rubric might be:</span></span>

| | <span data-ttu-id="45342-115">良好</span><span class="sxs-lookup"><span data-stu-id="45342-115">Good</span></span> | <span data-ttu-id="45342-116">较差</span><span class="sxs-lookup"><span data-stu-id="45342-116">Poor</span></span> |
|:--|:--|:--|
| <span data-ttu-id="45342-117">参数</span><span class="sxs-lookup"><span data-stu-id="45342-117">Argument</span></span> | <span data-ttu-id="45342-118">文章的参数具有说服力。</span><span class="sxs-lookup"><span data-stu-id="45342-118">The essay's argument is persuasive.</span></span> | <span data-ttu-id="45342-119">文章的参数毫无意义。</span><span class="sxs-lookup"><span data-stu-id="45342-119">The essay's argument does not make sense.</span></span> |
| <span data-ttu-id="45342-120">拼写和语法</span><span class="sxs-lookup"><span data-stu-id="45342-120">Tools > Spelling and Grammar </span></span> | <span data-ttu-id="45342-121">文章使用正确的拼写和语法，几乎没有或者完全没有错误。</span><span class="sxs-lookup"><span data-stu-id="45342-121">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="45342-122">文章中有许多拼写和/或语法错误。</span><span class="sxs-lookup"><span data-stu-id="45342-122">The essay has numerous errors in spelling and/or grammar.</span></span> |

<span data-ttu-id="45342-123">使用评分标准的评分涉及为评分标准中的每种*质量*选择一个*级别*。</span><span class="sxs-lookup"><span data-stu-id="45342-123">Grading using a rubric involves selecting one *level* for each *quality* in the rubric.</span></span>

<span data-ttu-id="45342-124">评分标准*可能*具有与每个级别关联的点数以及与每个质量关联的权重。</span><span class="sxs-lookup"><span data-stu-id="45342-124">A rubric *may* have points associated with each level, and a weight associated with each quality.</span></span>  <span data-ttu-id="45342-125">如果存在，权重加起来必须等于 100。</span><span class="sxs-lookup"><span data-stu-id="45342-125">If present, weights must add up to 100.</span></span>

| | <span data-ttu-id="45342-126">良好（2 点）</span><span class="sxs-lookup"><span data-stu-id="45342-126">Good (2 points)</span></span> | <span data-ttu-id="45342-127">较差（1 点）</span><span class="sxs-lookup"><span data-stu-id="45342-127">Poor (1 point)</span></span> |
|:--|:--|:--|
| <span data-ttu-id="45342-128">参数（权重 50）</span><span class="sxs-lookup"><span data-stu-id="45342-128">Argument (weight 50)</span></span> | <span data-ttu-id="45342-129">文章的参数具有说服力。</span><span class="sxs-lookup"><span data-stu-id="45342-129">The essay's argument is persuasive.</span></span> | <span data-ttu-id="45342-130">文章的参数毫无意义。</span><span class="sxs-lookup"><span data-stu-id="45342-130">The essay's argument does not make sense.</span></span> |
| <span data-ttu-id="45342-131">拼写和语法（权重 50）</span><span class="sxs-lookup"><span data-stu-id="45342-131">Spelling and Grammar (weight 50)</span></span> | <span data-ttu-id="45342-132">文章使用正确的拼写和语法，几乎没有或者完全没有错误。</span><span class="sxs-lookup"><span data-stu-id="45342-132">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="45342-133">文章中有许多拼写和/或语法错误。</span><span class="sxs-lookup"><span data-stu-id="45342-133">The essay has numerous errors in spelling and/or grammar.</span></span> |

## <a name="api-reference"></a><span data-ttu-id="45342-134">API 参考</span><span class="sxs-lookup"><span data-stu-id="45342-134">API reference</span></span>

<span data-ttu-id="45342-135">若要开始使用评分标准，请首先了解 [Microsoft Graph beta 中的 educationRubric 资源](/graph/api/resources/educationrubric?view=graph-rest-beta)及相关方法。</span><span class="sxs-lookup"><span data-stu-id="45342-135">To begin using rubrics, start with the [educationRubric resource in Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) and associated methods.</span></span>





 

