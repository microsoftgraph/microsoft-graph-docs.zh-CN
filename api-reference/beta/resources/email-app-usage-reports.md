---
title: 电子邮件应用使用情况报表
description: 您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 5a186638714057e461aa495e7e589984ae100c96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499713"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="bb2cb-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="bb2cb-104">Email app usage reports</span></span>

<span data-ttu-id="bb2cb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb2cb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb2cb-106">您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="bb2cb-107">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="bb2cb-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="bb2cb-109">报表</span><span class="sxs-lookup"><span data-stu-id="bb2cb-109">Reports</span></span>

| <span data-ttu-id="bb2cb-110">函数</span><span class="sxs-lookup"><span data-stu-id="bb2cb-110">Function</span></span>                                 | <span data-ttu-id="bb2cb-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="bb2cb-111">CSV return type</span></span> | <span data-ttu-id="bb2cb-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="bb2cb-112">JSON return type</span></span>                         | <span data-ttu-id="bb2cb-113">说明</span><span class="sxs-lookup"><span data-stu-id="bb2cb-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="bb2cb-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="bb2cb-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="bb2cb-115">Stream</span><span class="sxs-lookup"><span data-stu-id="bb2cb-115">Stream</span></span>          | [<span data-ttu-id="bb2cb-116">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="bb2cb-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="bb2cb-117">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="bb2cb-118">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="bb2cb-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="bb2cb-119">Stream</span><span class="sxs-lookup"><span data-stu-id="bb2cb-119">Stream</span></span>          | [<span data-ttu-id="bb2cb-120">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb2cb-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="bb2cb-121">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="bb2cb-122">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="bb2cb-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="bb2cb-123">Stream</span><span class="sxs-lookup"><span data-stu-id="bb2cb-123">Stream</span></span>          | [<span data-ttu-id="bb2cb-124">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb2cb-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="bb2cb-125">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="bb2cb-126">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="bb2cb-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="bb2cb-127">Stream</span><span class="sxs-lookup"><span data-stu-id="bb2cb-127">Stream</span></span>          | [<span data-ttu-id="bb2cb-128">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb2cb-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="bb2cb-129">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-129">Get the count of unique users by Outlook desktop version.</span></span> |
