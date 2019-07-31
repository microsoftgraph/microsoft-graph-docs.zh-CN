---
title: Yammer 活动报表
description: 您可以通过在组织中生成多少活动以及在 Yammer 上进行 post (如和阅读邮件) 的唯一用户的数量来了解您的组织对 Yammer 的服务级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: efdb4ba603be33f18cd66529edd724f6e1a3798d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963827"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="73836-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="73836-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73836-104">您可以通过在组织中生成多少活动以及在 Yammer 上进行 post (如和阅读邮件) 的唯一用户的数量来了解您的组织对 Yammer 的服务级别。</span><span class="sxs-lookup"><span data-stu-id="73836-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="73836-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="73836-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="73836-106">报表</span><span class="sxs-lookup"><span data-stu-id="73836-106">Reports</span></span>

| <span data-ttu-id="73836-107">函数</span><span class="sxs-lookup"><span data-stu-id="73836-107">Function</span></span>                                 | <span data-ttu-id="73836-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="73836-108">CSV return type</span></span> | <span data-ttu-id="73836-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="73836-109">JSON return type</span></span>                         | <span data-ttu-id="73836-110">说明</span><span class="sxs-lookup"><span data-stu-id="73836-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="73836-111">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="73836-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="73836-112">流</span><span class="sxs-lookup"><span data-stu-id="73836-112">Stream</span></span>          | [<span data-ttu-id="73836-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="73836-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="73836-114">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="73836-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="73836-115">获取活动数</span><span class="sxs-lookup"><span data-stu-id="73836-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="73836-116">Stream</span><span class="sxs-lookup"><span data-stu-id="73836-116">Stream</span></span>          | [<span data-ttu-id="73836-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="73836-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="73836-118">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="73836-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="73836-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="73836-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="73836-120">Stream</span><span class="sxs-lookup"><span data-stu-id="73836-120">Stream</span></span>          | [<span data-ttu-id="73836-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="73836-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="73836-122">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="73836-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
