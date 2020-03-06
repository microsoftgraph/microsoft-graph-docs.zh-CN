---
title: Yammer 活动报表
description: Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: b6f92ba4745d69cf2ce341412eee88403218414c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533357"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="a50c6-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="a50c6-103">Yammer activity reports</span></span>

<span data-ttu-id="a50c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a50c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a50c6-105">Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。</span><span class="sxs-lookup"><span data-stu-id="a50c6-105">You can use the Yammer activity reports to understand the level of your organization's engagement with Yammer by seeing how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="a50c6-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="a50c6-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="a50c6-107">报表</span><span class="sxs-lookup"><span data-stu-id="a50c6-107">Reports</span></span>

| <span data-ttu-id="a50c6-108">函数</span><span class="sxs-lookup"><span data-stu-id="a50c6-108">Function</span></span>                                 | <span data-ttu-id="a50c6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a50c6-109">Return Type</span></span> | <span data-ttu-id="a50c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="a50c6-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="a50c6-111">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="a50c6-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="a50c6-112">Stream</span><span class="sxs-lookup"><span data-stu-id="a50c6-112">Stream</span></span>      | <span data-ttu-id="a50c6-113">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a50c6-113">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="a50c6-114">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="a50c6-114">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="a50c6-115">Stream</span><span class="sxs-lookup"><span data-stu-id="a50c6-115">Stream</span></span>      | <span data-ttu-id="a50c6-116">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="a50c6-116">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="a50c6-117">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="a50c6-117">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="a50c6-118">Stream</span><span class="sxs-lookup"><span data-stu-id="a50c6-118">Stream</span></span>      | <span data-ttu-id="a50c6-119">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="a50c6-119">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
