---
title: Yammer 活动报表
description: 您可以通过在组织中生成多少活动以及在 yammer 上进行 post (如和阅读邮件) 的唯一用户的数量来了解您的组织对 yammer 的服务级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 792b639a2f843a0b902b3a153eee16da3c0b3b76
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342773"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="64ce6-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="64ce6-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64ce6-104">您可以通过在组织中生成多少活动以及在 yammer 上进行 post (如和阅读邮件) 的唯一用户的数量来了解您的组织对 yammer 的服务级别。</span><span class="sxs-lookup"><span data-stu-id="64ce6-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="64ce6-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="64ce6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="64ce6-106">报表</span><span class="sxs-lookup"><span data-stu-id="64ce6-106">Reports</span></span>

| <span data-ttu-id="64ce6-107">函数</span><span class="sxs-lookup"><span data-stu-id="64ce6-107">Function</span></span>                                 | <span data-ttu-id="64ce6-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="64ce6-108">CSV return type</span></span> | <span data-ttu-id="64ce6-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="64ce6-109">JSON return type</span></span>                         | <span data-ttu-id="64ce6-110">说明</span><span class="sxs-lookup"><span data-stu-id="64ce6-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="64ce6-111">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="64ce6-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="64ce6-112">Stream</span><span class="sxs-lookup"><span data-stu-id="64ce6-112">Stream</span></span>          | [<span data-ttu-id="64ce6-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="64ce6-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="64ce6-114">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="64ce6-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="64ce6-115">获取活动数</span><span class="sxs-lookup"><span data-stu-id="64ce6-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="64ce6-116">Stream</span><span class="sxs-lookup"><span data-stu-id="64ce6-116">Stream</span></span>          | [<span data-ttu-id="64ce6-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="64ce6-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="64ce6-118">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="64ce6-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="64ce6-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="64ce6-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="64ce6-120">Stream</span><span class="sxs-lookup"><span data-stu-id="64ce6-120">Stream</span></span>          | [<span data-ttu-id="64ce6-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="64ce6-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="64ce6-122">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="64ce6-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
