---
title: Yammer 活动报表
description: 您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 69c155df86cfe772e0c065bec0297a83fb7f3a8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912034"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="0aff1-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="0aff1-103">Yammer activity reports</span></span>

> <span data-ttu-id="0aff1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0aff1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0aff1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0aff1-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="0aff1-106">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="0aff1-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="0aff1-107">您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。</span><span class="sxs-lookup"><span data-stu-id="0aff1-107">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="0aff1-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="0aff1-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="0aff1-109">报表</span><span class="sxs-lookup"><span data-stu-id="0aff1-109">Reports</span></span>

| <span data-ttu-id="0aff1-110">函数</span><span class="sxs-lookup"><span data-stu-id="0aff1-110">Function</span></span>                                 | <span data-ttu-id="0aff1-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="0aff1-111">CSV return type</span></span> | <span data-ttu-id="0aff1-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="0aff1-112">JSON return type</span></span>                         | <span data-ttu-id="0aff1-113">说明</span><span class="sxs-lookup"><span data-stu-id="0aff1-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0aff1-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="0aff1-114">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="0aff1-115">Stream</span><span class="sxs-lookup"><span data-stu-id="0aff1-115">Stream</span></span>          | [<span data-ttu-id="0aff1-116">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0aff1-116">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="0aff1-117">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0aff1-117">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="0aff1-118">获取活动数</span><span class="sxs-lookup"><span data-stu-id="0aff1-118">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="0aff1-119">Stream</span><span class="sxs-lookup"><span data-stu-id="0aff1-119">Stream</span></span>          | [<span data-ttu-id="0aff1-120">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="0aff1-120">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="0aff1-121">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="0aff1-121">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="0aff1-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="0aff1-122">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="0aff1-123">Stream</span><span class="sxs-lookup"><span data-stu-id="0aff1-123">Stream</span></span>          | [<span data-ttu-id="0aff1-124">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="0aff1-124">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="0aff1-125">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="0aff1-125">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
