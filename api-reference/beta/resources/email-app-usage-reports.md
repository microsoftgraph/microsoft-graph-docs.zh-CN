---
title: 电子邮件应用使用情况报表
description: 您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: df40e61108a3933801f5e7c21057f71600b496ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340188"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="4f336-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="4f336-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f336-105">您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="4f336-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="4f336-106">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="4f336-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="4f336-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="4f336-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="4f336-108">报表</span><span class="sxs-lookup"><span data-stu-id="4f336-108">Reports</span></span>

| <span data-ttu-id="4f336-109">函数</span><span class="sxs-lookup"><span data-stu-id="4f336-109">Function</span></span>                                 | <span data-ttu-id="4f336-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="4f336-110">CSV return type</span></span> | <span data-ttu-id="4f336-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="4f336-111">JSON return type</span></span>                         | <span data-ttu-id="4f336-112">说明</span><span class="sxs-lookup"><span data-stu-id="4f336-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4f336-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="4f336-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="4f336-114">Stream</span><span class="sxs-lookup"><span data-stu-id="4f336-114">Stream</span></span>          | [<span data-ttu-id="4f336-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="4f336-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="4f336-116">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4f336-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="4f336-117">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="4f336-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="4f336-118">Stream</span><span class="sxs-lookup"><span data-stu-id="4f336-118">Stream</span></span>          | [<span data-ttu-id="4f336-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f336-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="4f336-120">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="4f336-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="4f336-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="4f336-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="4f336-122">Stream</span><span class="sxs-lookup"><span data-stu-id="4f336-122">Stream</span></span>          | [<span data-ttu-id="4f336-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f336-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="4f336-124">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="4f336-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="4f336-125">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="4f336-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="4f336-126">Stream</span><span class="sxs-lookup"><span data-stu-id="4f336-126">Stream</span></span>          | [<span data-ttu-id="4f336-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f336-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="4f336-128">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="4f336-128">Get the count of unique users by Outlook desktop version.</span></span> |
