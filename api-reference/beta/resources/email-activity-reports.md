---
title: 电子邮件活动报表
description: 可以从"报告"页获取组织中电子邮件流量的高级别视图。 还可以深入了解"电子邮件活动"小部件，了解组织中电子邮件活动的每个用户的趋势和详细信息。
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: db9ea032b418a6beca7afb7c15eb16b762e6ed11
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983795"
---
# <a name="email-activity-reports"></a><span data-ttu-id="e75ef-104">电子邮件活动报告</span><span class="sxs-lookup"><span data-stu-id="e75ef-104">Email activity reports</span></span>

<span data-ttu-id="e75ef-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e75ef-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e75ef-106">可以从"报告"页获取组织中电子邮件流量的高级别视图。</span><span class="sxs-lookup"><span data-stu-id="e75ef-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="e75ef-107">还可以深入了解"电子邮件活动"小部件，了解组织中电子邮件活动的每个用户的趋势和详细信息。</span><span class="sxs-lookup"><span data-stu-id="e75ef-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="e75ef-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱活动况](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="e75ef-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="e75ef-109">报告</span><span class="sxs-lookup"><span data-stu-id="e75ef-109">Reports</span></span>

| <span data-ttu-id="e75ef-110">函数</span><span class="sxs-lookup"><span data-stu-id="e75ef-110">Function</span></span>                                 | <span data-ttu-id="e75ef-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="e75ef-111">CSV return type</span></span> | <span data-ttu-id="e75ef-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="e75ef-112">JSON return type</span></span>                         | <span data-ttu-id="e75ef-113">说明</span><span class="sxs-lookup"><span data-stu-id="e75ef-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e75ef-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="e75ef-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="e75ef-115">Stream</span><span class="sxs-lookup"><span data-stu-id="e75ef-115">Stream</span></span>          | [<span data-ttu-id="e75ef-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e75ef-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="e75ef-117">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e75ef-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="e75ef-118">获取活动数</span><span class="sxs-lookup"><span data-stu-id="e75ef-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="e75ef-119">Stream</span><span class="sxs-lookup"><span data-stu-id="e75ef-119">Stream</span></span>          | [<span data-ttu-id="e75ef-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e75ef-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="e75ef-121">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="e75ef-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="e75ef-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e75ef-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="e75ef-123">Stream</span><span class="sxs-lookup"><span data-stu-id="e75ef-123">Stream</span></span>          | [<span data-ttu-id="e75ef-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e75ef-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="e75ef-125">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="e75ef-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |


