---
title: 教育版评分标准概述
description: 评分标准是一种被广泛采用的有效作业评分方式，Microsoft Graph 中的教育版 API 支持它们。
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: d17b325c12c75fbdd54d17a293aa6352707666e3
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845482"
---
# <a name="education-rubric-overview"></a><span data-ttu-id="234fc-103">教育版评分标准概述</span><span class="sxs-lookup"><span data-stu-id="234fc-103">Education rubric overview</span></span>

<span data-ttu-id="234fc-104">评分标准是一种被广泛采用的有效作业评分方式，Microsoft Graph 中的教育版 API 支持它们。</span><span class="sxs-lookup"><span data-stu-id="234fc-104">Rubrics are an effective and widely-used way of grading assignments, and the education API in Microsoft Graph supports them.</span></span>

<span data-ttu-id="234fc-105">评分标准是一个*质量*、*级别*和*条件*矩阵，如下所示：</span><span class="sxs-lookup"><span data-stu-id="234fc-105">A grading rubric is a matrix of *qualities*, *levels*, and *criteria*, as follows:</span></span>

| &nbsp;  | <span data-ttu-id="234fc-106">级别</span><span class="sxs-lookup"><span data-stu-id="234fc-106">Level</span></span>     | <span data-ttu-id="234fc-107">级别</span><span class="sxs-lookup"><span data-stu-id="234fc-107">Level</span></span>     |
|:--------|:----------|:----------|
| <span data-ttu-id="234fc-108">质量</span><span class="sxs-lookup"><span data-stu-id="234fc-108">Quality</span></span> | <span data-ttu-id="234fc-109">条件</span><span class="sxs-lookup"><span data-stu-id="234fc-109">Criterion</span></span> | <span data-ttu-id="234fc-110">条件</span><span class="sxs-lookup"><span data-stu-id="234fc-110">Criterion</span></span> |
| <span data-ttu-id="234fc-111">质量</span><span class="sxs-lookup"><span data-stu-id="234fc-111">Quality</span></span> | <span data-ttu-id="234fc-112">条件</span><span class="sxs-lookup"><span data-stu-id="234fc-112">Criterion</span></span> | <span data-ttu-id="234fc-113">条件</span><span class="sxs-lookup"><span data-stu-id="234fc-113">Criterion</span></span> |

<span data-ttu-id="234fc-114">评分标准示例如下：</span><span class="sxs-lookup"><span data-stu-id="234fc-114">An example of a grading rubric might be:</span></span>

| &nbsp;               | <span data-ttu-id="234fc-115">良好</span><span class="sxs-lookup"><span data-stu-id="234fc-115">Good</span></span>                                                              | <span data-ttu-id="234fc-116">较差</span><span class="sxs-lookup"><span data-stu-id="234fc-116">Poor</span></span>                                                      |
|:---------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="234fc-117">参数</span><span class="sxs-lookup"><span data-stu-id="234fc-117">Argument</span></span>             | <span data-ttu-id="234fc-118">文章的参数具有说服力。</span><span class="sxs-lookup"><span data-stu-id="234fc-118">The essay's argument is persuasive.</span></span>                               | <span data-ttu-id="234fc-119">文章的参数毫无意义。</span><span class="sxs-lookup"><span data-stu-id="234fc-119">The essay's argument does not make sense.</span></span>                 |
| <span data-ttu-id="234fc-120">拼写和语法</span><span class="sxs-lookup"><span data-stu-id="234fc-120">Spelling and Grammar</span></span> | <span data-ttu-id="234fc-121">文章使用正确的拼写和语法，几乎没有或者完全没有错误。</span><span class="sxs-lookup"><span data-stu-id="234fc-121">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="234fc-122">文章中有许多拼写和/或语法错误。</span><span class="sxs-lookup"><span data-stu-id="234fc-122">The essay has numerous errors in spelling and/or grammar.</span></span> |

<span data-ttu-id="234fc-123">使用评分标准的评分涉及为评分标准中的每种*质量*选择一个*级别*。</span><span class="sxs-lookup"><span data-stu-id="234fc-123">Grading using a rubric involves selecting one *level* for each *quality* in the rubric.</span></span>

<span data-ttu-id="234fc-124">评分标准*可能*具有与每个级别关联的点数以及与每个质量关联的权重。</span><span class="sxs-lookup"><span data-stu-id="234fc-124">A rubric *may* have points associated with each level, and a weight associated with each quality.</span></span>  <span data-ttu-id="234fc-125">如果存在，权重加起来必须等于 100。</span><span class="sxs-lookup"><span data-stu-id="234fc-125">If present, weights must add up to 100.</span></span>

| &nbsp;                           | <span data-ttu-id="234fc-126">良好（2 点）</span><span class="sxs-lookup"><span data-stu-id="234fc-126">Good (2 points)</span></span>                                                   | <span data-ttu-id="234fc-127">较差（1 点）</span><span class="sxs-lookup"><span data-stu-id="234fc-127">Poor (1 point)</span></span>                                            |
|:---------------------------------|:------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="234fc-128">参数（权重 50）</span><span class="sxs-lookup"><span data-stu-id="234fc-128">Argument (weight 50)</span></span>             | <span data-ttu-id="234fc-129">文章的参数具有说服力。</span><span class="sxs-lookup"><span data-stu-id="234fc-129">The essay's argument is persuasive.</span></span>                               | <span data-ttu-id="234fc-130">文章的参数毫无意义。</span><span class="sxs-lookup"><span data-stu-id="234fc-130">The essay's argument does not make sense.</span></span>                 |
| <span data-ttu-id="234fc-131">拼写和语法（权重 50）</span><span class="sxs-lookup"><span data-stu-id="234fc-131">Spelling and Grammar (weight 50)</span></span> | <span data-ttu-id="234fc-132">文章使用正确的拼写和语法，几乎没有或者完全没有错误。</span><span class="sxs-lookup"><span data-stu-id="234fc-132">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="234fc-133">文章中有许多拼写和/或语法错误。</span><span class="sxs-lookup"><span data-stu-id="234fc-133">The essay has numerous errors in spelling and/or grammar.</span></span> |

## <a name="api-reference"></a><span data-ttu-id="234fc-134">API 参考</span><span class="sxs-lookup"><span data-stu-id="234fc-134">API reference</span></span>

<span data-ttu-id="234fc-135">若要开始使用评分标准，请首先了解 [Microsoft Graph beta 中的 educationRubric 资源](/graph/api/resources/educationrubric?view=graph-rest-beta)及相关方法。</span><span class="sxs-lookup"><span data-stu-id="234fc-135">To begin using rubrics, start with the [educationRubric resource in Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) and associated methods.</span></span>
