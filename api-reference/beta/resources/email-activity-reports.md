---
title: 电子邮件活动报表
description: 您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。 您还可以深入了解电子邮件活动小组件，以了解组织中的电子邮件活动的每个用户的趋势和详细信息。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 7dcfaf2d5cc2d1dbd38cdc4a8a7c5eac71e9539b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499804"
---
# <a name="email-activity-reports"></a><span data-ttu-id="2a8fb-104">电子邮件活动报告</span><span class="sxs-lookup"><span data-stu-id="2a8fb-104">Email activity reports</span></span>

<span data-ttu-id="2a8fb-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2a8fb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a8fb-106">您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。</span><span class="sxs-lookup"><span data-stu-id="2a8fb-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="2a8fb-107">您还可以深入了解电子邮件活动小组件，以了解组织中的电子邮件活动的每个用户的趋势和详细信息。</span><span class="sxs-lookup"><span data-stu-id="2a8fb-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="2a8fb-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="2a8fb-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="2a8fb-109">报表</span><span class="sxs-lookup"><span data-stu-id="2a8fb-109">Reports</span></span>

| <span data-ttu-id="2a8fb-110">函数</span><span class="sxs-lookup"><span data-stu-id="2a8fb-110">Function</span></span>                                 | <span data-ttu-id="2a8fb-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="2a8fb-111">CSV return type</span></span> | <span data-ttu-id="2a8fb-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="2a8fb-112">JSON return type</span></span>                         | <span data-ttu-id="2a8fb-113">说明</span><span class="sxs-lookup"><span data-stu-id="2a8fb-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2a8fb-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="2a8fb-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="2a8fb-115">Stream</span><span class="sxs-lookup"><span data-stu-id="2a8fb-115">Stream</span></span>          | [<span data-ttu-id="2a8fb-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2a8fb-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="2a8fb-117">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2a8fb-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="2a8fb-118">获取活动数</span><span class="sxs-lookup"><span data-stu-id="2a8fb-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="2a8fb-119">Stream</span><span class="sxs-lookup"><span data-stu-id="2a8fb-119">Stream</span></span>          | [<span data-ttu-id="2a8fb-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2a8fb-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="2a8fb-121">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="2a8fb-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="2a8fb-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="2a8fb-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="2a8fb-123">Stream</span><span class="sxs-lookup"><span data-stu-id="2a8fb-123">Stream</span></span>          | [<span data-ttu-id="2a8fb-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2a8fb-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="2a8fb-125">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="2a8fb-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
