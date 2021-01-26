---
title: Yammer 活动报表
description: Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 739952680d4996fc259ccc9edf278469066048d9
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980596"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="4f42f-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="4f42f-103">Yammer activity reports</span></span>

<span data-ttu-id="4f42f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f42f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f42f-105">Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。</span><span class="sxs-lookup"><span data-stu-id="4f42f-105">You can use the Yammer activity reports to understand the level of your organization's engagement with Yammer by seeing how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="4f42f-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="4f42f-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="4f42f-107">报告</span><span class="sxs-lookup"><span data-stu-id="4f42f-107">Reports</span></span>

| <span data-ttu-id="4f42f-108">函数</span><span class="sxs-lookup"><span data-stu-id="4f42f-108">Function</span></span>                                 | <span data-ttu-id="4f42f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f42f-109">Return Type</span></span> | <span data-ttu-id="4f42f-110">说明</span><span class="sxs-lookup"><span data-stu-id="4f42f-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="4f42f-111">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="4f42f-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="4f42f-112">Stream</span><span class="sxs-lookup"><span data-stu-id="4f42f-112">Stream</span></span>      | <span data-ttu-id="4f42f-113">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4f42f-113">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="4f42f-114">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="4f42f-114">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="4f42f-115">Stream</span><span class="sxs-lookup"><span data-stu-id="4f42f-115">Stream</span></span>      | <span data-ttu-id="4f42f-116">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="4f42f-116">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="4f42f-117">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="4f42f-117">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="4f42f-118">Stream</span><span class="sxs-lookup"><span data-stu-id="4f42f-118">Stream</span></span>      | <span data-ttu-id="4f42f-119">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="4f42f-119">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |

