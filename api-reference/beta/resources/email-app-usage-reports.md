---
title: 电子邮件应用使用情况报表
description: 你可以看到有多少电子邮件应用用于连接到 Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: efa7a747ae26da8f34c32d9473a84f95b7433ee0
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982703"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="221f4-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="221f4-104">Email app usage reports</span></span>

<span data-ttu-id="221f4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="221f4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="221f4-106">你可以看到有多少电子邮件应用用于连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="221f4-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="221f4-107">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="221f4-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="221f4-108">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报告 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="221f4-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="221f4-109">报告</span><span class="sxs-lookup"><span data-stu-id="221f4-109">Reports</span></span>

| <span data-ttu-id="221f4-110">函数</span><span class="sxs-lookup"><span data-stu-id="221f4-110">Function</span></span>                                 | <span data-ttu-id="221f4-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="221f4-111">CSV return type</span></span> | <span data-ttu-id="221f4-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="221f4-112">JSON return type</span></span>                         | <span data-ttu-id="221f4-113">说明</span><span class="sxs-lookup"><span data-stu-id="221f4-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="221f4-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="221f4-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="221f4-115">Stream</span><span class="sxs-lookup"><span data-stu-id="221f4-115">Stream</span></span>          | [<span data-ttu-id="221f4-116">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="221f4-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="221f4-117">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="221f4-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="221f4-118">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="221f4-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="221f4-119">Stream</span><span class="sxs-lookup"><span data-stu-id="221f4-119">Stream</span></span>          | [<span data-ttu-id="221f4-120">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="221f4-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="221f4-121">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="221f4-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="221f4-122">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="221f4-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="221f4-123">Stream</span><span class="sxs-lookup"><span data-stu-id="221f4-123">Stream</span></span>          | [<span data-ttu-id="221f4-124">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="221f4-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="221f4-125">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="221f4-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="221f4-126">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="221f4-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="221f4-127">Stream</span><span class="sxs-lookup"><span data-stu-id="221f4-127">Stream</span></span>          | [<span data-ttu-id="221f4-128">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="221f4-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="221f4-129">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="221f4-129">Get the count of unique users by Outlook desktop version.</span></span> |


