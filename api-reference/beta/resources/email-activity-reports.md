---
title: 电子邮件活动报表
description: 您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。 您还可以深入了解电子邮件活动小组件, 以了解组织中的电子邮件活动的每个用户的趋势和详细信息。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 748199a2e846cc71a3f04c3ea1bda97dcf2c7301
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542901"
---
# <a name="email-activity-reports"></a><span data-ttu-id="dd94b-104">电子邮件活动报告</span><span class="sxs-lookup"><span data-stu-id="dd94b-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd94b-105">您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。</span><span class="sxs-lookup"><span data-stu-id="dd94b-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="dd94b-106">您还可以深入了解电子邮件活动小组件, 以了解组织中的电子邮件活动的每个用户的趋势和详细信息。</span><span class="sxs-lookup"><span data-stu-id="dd94b-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="dd94b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="dd94b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="dd94b-108">报表</span><span class="sxs-lookup"><span data-stu-id="dd94b-108">Reports</span></span>

| <span data-ttu-id="dd94b-109">函数</span><span class="sxs-lookup"><span data-stu-id="dd94b-109">Function</span></span>                                 | <span data-ttu-id="dd94b-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="dd94b-110">CSV return type</span></span> | <span data-ttu-id="dd94b-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="dd94b-111">JSON return type</span></span>                         | <span data-ttu-id="dd94b-112">说明</span><span class="sxs-lookup"><span data-stu-id="dd94b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="dd94b-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="dd94b-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="dd94b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="dd94b-114">Stream</span></span>          | [<span data-ttu-id="dd94b-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="dd94b-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="dd94b-116">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dd94b-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="dd94b-117">获取活动数</span><span class="sxs-lookup"><span data-stu-id="dd94b-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="dd94b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="dd94b-118">Stream</span></span>          | [<span data-ttu-id="dd94b-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="dd94b-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="dd94b-120">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="dd94b-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="dd94b-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="dd94b-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="dd94b-122">Stream</span><span class="sxs-lookup"><span data-stu-id="dd94b-122">Stream</span></span>          | [<span data-ttu-id="dd94b-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="dd94b-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="dd94b-124">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="dd94b-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
