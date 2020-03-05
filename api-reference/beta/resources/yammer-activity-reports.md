---
title: Yammer 活动报表
description: 您可以通过在组织中生成多少活动以及在 Yammer 上进行 post （如和阅读邮件）的唯一用户的数量来了解您的组织对 Yammer 的服务级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 8f1358c188b06953d7af180c2b7ad83b6183af35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519055"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="b2d83-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="b2d83-103">Yammer activity reports</span></span>

<span data-ttu-id="b2d83-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b2d83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d83-105">您可以通过在组织中生成多少活动以及在 Yammer 上进行 post （如和阅读邮件）的唯一用户的数量来了解您的组织对 Yammer 的服务级别。</span><span class="sxs-lookup"><span data-stu-id="b2d83-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="b2d83-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="b2d83-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="b2d83-107">报表</span><span class="sxs-lookup"><span data-stu-id="b2d83-107">Reports</span></span>

| <span data-ttu-id="b2d83-108">函数</span><span class="sxs-lookup"><span data-stu-id="b2d83-108">Function</span></span>                                 | <span data-ttu-id="b2d83-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="b2d83-109">CSV return type</span></span> | <span data-ttu-id="b2d83-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="b2d83-110">JSON return type</span></span>                         | <span data-ttu-id="b2d83-111">说明</span><span class="sxs-lookup"><span data-stu-id="b2d83-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b2d83-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="b2d83-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="b2d83-113">Stream</span><span class="sxs-lookup"><span data-stu-id="b2d83-113">Stream</span></span>          | [<span data-ttu-id="b2d83-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b2d83-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="b2d83-115">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b2d83-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="b2d83-116">获取活动数</span><span class="sxs-lookup"><span data-stu-id="b2d83-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="b2d83-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b2d83-117">Stream</span></span>          | [<span data-ttu-id="b2d83-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="b2d83-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="b2d83-119">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="b2d83-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="b2d83-120">获取用户数</span><span class="sxs-lookup"><span data-stu-id="b2d83-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="b2d83-121">Stream</span><span class="sxs-lookup"><span data-stu-id="b2d83-121">Stream</span></span>          | [<span data-ttu-id="b2d83-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="b2d83-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="b2d83-123">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="b2d83-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
