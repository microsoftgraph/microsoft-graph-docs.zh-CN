---
title: 电子邮件活动报表
description: 您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。 您还可以深入了解电子邮件活动小组件，以了解组织中的电子邮件活动的每个用户的趋势和详细信息。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 5f26498a0837993fc052cb536acd8bcd08f77ee1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896908"
---
# <a name="email-activity-reports"></a><span data-ttu-id="ab359-104">电子邮件活动报告</span><span class="sxs-lookup"><span data-stu-id="ab359-104">Email activity reports</span></span>

<span data-ttu-id="ab359-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab359-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab359-106">您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。</span><span class="sxs-lookup"><span data-stu-id="ab359-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="ab359-107">您还可以深入了解电子邮件活动小组件，以了解组织中的电子邮件活动的每个用户的趋势和详细信息。</span><span class="sxs-lookup"><span data-stu-id="ab359-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="ab359-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="ab359-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="ab359-109">报表</span><span class="sxs-lookup"><span data-stu-id="ab359-109">Reports</span></span>

| <span data-ttu-id="ab359-110">函数</span><span class="sxs-lookup"><span data-stu-id="ab359-110">Function</span></span>                                 | <span data-ttu-id="ab359-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="ab359-111">CSV return type</span></span> | <span data-ttu-id="ab359-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="ab359-112">JSON return type</span></span>                         | <span data-ttu-id="ab359-113">说明</span><span class="sxs-lookup"><span data-stu-id="ab359-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ab359-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="ab359-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="ab359-115">Stream</span><span class="sxs-lookup"><span data-stu-id="ab359-115">Stream</span></span>          | [<span data-ttu-id="ab359-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ab359-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="ab359-117">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ab359-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="ab359-118">获取活动数</span><span class="sxs-lookup"><span data-stu-id="ab359-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="ab359-119">Stream</span><span class="sxs-lookup"><span data-stu-id="ab359-119">Stream</span></span>          | [<span data-ttu-id="ab359-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ab359-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="ab359-121">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="ab359-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="ab359-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="ab359-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="ab359-123">Stream</span><span class="sxs-lookup"><span data-stu-id="ab359-123">Stream</span></span>          | [<span data-ttu-id="ab359-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ab359-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="ab359-125">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="ab359-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
