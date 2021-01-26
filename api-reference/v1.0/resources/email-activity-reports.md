---
title: 电子邮件活动报表
description: 电子邮件活动报表可用于大致了解组织中的电子邮件流量。 此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。
localization_priority: Priority
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 7f0716d42d9b3e2f2fa360e065ebfd9ed7e1a4fc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982941"
---
# <a name="email-activity-reports"></a><span data-ttu-id="42065-104">电子邮件活动报告</span><span class="sxs-lookup"><span data-stu-id="42065-104">Email activity reports</span></span>

<span data-ttu-id="42065-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42065-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42065-106">电子邮件活动报表可用于大致了解组织中的电子邮件流量。</span><span class="sxs-lookup"><span data-stu-id="42065-106">Use the email activity reports to get a high level view of email traffic within your organization.</span></span> <span data-ttu-id="42065-107">此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。</span><span class="sxs-lookup"><span data-stu-id="42065-107">You can also drill into the Email Activity widget to understand the trends and details of the email activity per user in your organization.</span></span>

> <span data-ttu-id="42065-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱活动况](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="42065-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="42065-109">报告</span><span class="sxs-lookup"><span data-stu-id="42065-109">Reports</span></span>

| <span data-ttu-id="42065-110">函数</span><span class="sxs-lookup"><span data-stu-id="42065-110">Function</span></span>                                 | <span data-ttu-id="42065-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="42065-111">Return Type</span></span> | <span data-ttu-id="42065-112">说明</span><span class="sxs-lookup"><span data-stu-id="42065-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="42065-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="42065-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="42065-114">Stream</span><span class="sxs-lookup"><span data-stu-id="42065-114">Stream</span></span>      | <span data-ttu-id="42065-115">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="42065-115">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="42065-116">获取活动数</span><span class="sxs-lookup"><span data-stu-id="42065-116">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="42065-117">Stream</span><span class="sxs-lookup"><span data-stu-id="42065-117">Stream</span></span>      | <span data-ttu-id="42065-118">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="42065-118">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="42065-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="42065-119">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="42065-120">Stream</span><span class="sxs-lookup"><span data-stu-id="42065-120">Stream</span></span>      | <span data-ttu-id="42065-121">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="42065-121">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |

