---
title: 电子邮件活动报表
description: 电子邮件活动报表可用于大致了解组织中的电子邮件流量。 此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 861e206e2f63a314c551f8242d9fc20cc002064d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463899"
---
# <a name="email-activity-reports"></a><span data-ttu-id="bdd2d-104">电子邮件活动报告</span><span class="sxs-lookup"><span data-stu-id="bdd2d-104">Email activity reports</span></span>

<span data-ttu-id="bdd2d-105">电子邮件活动报表可用于大致了解组织中的电子邮件流量。</span><span class="sxs-lookup"><span data-stu-id="bdd2d-105">Use the email activity reports to get a high level view of email traffic within your organization.</span></span> <span data-ttu-id="bdd2d-106">此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdd2d-106">You can also drill into the Email Activity widget to understand the trends and details of the email activity per user in your organization.</span></span>

> <span data-ttu-id="bdd2d-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="bdd2d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="bdd2d-108">报表</span><span class="sxs-lookup"><span data-stu-id="bdd2d-108">Reports</span></span>

| <span data-ttu-id="bdd2d-109">函数</span><span class="sxs-lookup"><span data-stu-id="bdd2d-109">Function</span></span>                                 | <span data-ttu-id="bdd2d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bdd2d-110">Return Type</span></span> | <span data-ttu-id="bdd2d-111">说明</span><span class="sxs-lookup"><span data-stu-id="bdd2d-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="bdd2d-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="bdd2d-112">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="bdd2d-113">Stream</span><span class="sxs-lookup"><span data-stu-id="bdd2d-113">Stream</span></span>      | <span data-ttu-id="bdd2d-114">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdd2d-114">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="bdd2d-115">获取活动数</span><span class="sxs-lookup"><span data-stu-id="bdd2d-115">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="bdd2d-116">Stream</span><span class="sxs-lookup"><span data-stu-id="bdd2d-116">Stream</span></span>      | <span data-ttu-id="bdd2d-117">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="bdd2d-117">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="bdd2d-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="bdd2d-118">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="bdd2d-119">Stream</span><span class="sxs-lookup"><span data-stu-id="bdd2d-119">Stream</span></span>      | <span data-ttu-id="bdd2d-120">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="bdd2d-120">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
