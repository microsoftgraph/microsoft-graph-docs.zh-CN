---
title: Yammer 活动报表
description: 通过跨组织生成的活动量以及发布、喜欢和阅读 Yammer 上的消息的唯一用户数，您可以了解组织与 Yammer 的交互程度。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c0009949b5eb429f15155059768365b201078134
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982465"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="15b2d-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="15b2d-103">Yammer activity reports</span></span>

<span data-ttu-id="15b2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15b2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15b2d-105">通过跨组织生成的活动量以及发布、喜欢和阅读 Yammer 上的消息的唯一用户数，您可以了解组织与 Yammer 的交互程度。</span><span class="sxs-lookup"><span data-stu-id="15b2d-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="15b2d-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="15b2d-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="15b2d-107">报告</span><span class="sxs-lookup"><span data-stu-id="15b2d-107">Reports</span></span>

| <span data-ttu-id="15b2d-108">函数</span><span class="sxs-lookup"><span data-stu-id="15b2d-108">Function</span></span>                                 | <span data-ttu-id="15b2d-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="15b2d-109">CSV return type</span></span> | <span data-ttu-id="15b2d-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="15b2d-110">JSON return type</span></span>                         | <span data-ttu-id="15b2d-111">说明</span><span class="sxs-lookup"><span data-stu-id="15b2d-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="15b2d-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="15b2d-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="15b2d-113">Stream</span><span class="sxs-lookup"><span data-stu-id="15b2d-113">Stream</span></span>          | [<span data-ttu-id="15b2d-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="15b2d-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="15b2d-115">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="15b2d-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="15b2d-116">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="15b2d-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="15b2d-117">Stream</span><span class="sxs-lookup"><span data-stu-id="15b2d-117">Stream</span></span>          | [<span data-ttu-id="15b2d-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="15b2d-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="15b2d-119">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="15b2d-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="15b2d-120">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="15b2d-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="15b2d-121">Stream</span><span class="sxs-lookup"><span data-stu-id="15b2d-121">Stream</span></span>          | [<span data-ttu-id="15b2d-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="15b2d-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="15b2d-123">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="15b2d-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |


