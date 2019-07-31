---
title: 电子邮件应用使用情况报表
description: 您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: b7aeac4800fbd7681b60210e7f65c96e7086705c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972255"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="df111-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="df111-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df111-105">您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="df111-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="df111-106">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="df111-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="df111-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="df111-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="df111-108">报表</span><span class="sxs-lookup"><span data-stu-id="df111-108">Reports</span></span>

| <span data-ttu-id="df111-109">函数</span><span class="sxs-lookup"><span data-stu-id="df111-109">Function</span></span>                                 | <span data-ttu-id="df111-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="df111-110">CSV return type</span></span> | <span data-ttu-id="df111-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="df111-111">JSON return type</span></span>                         | <span data-ttu-id="df111-112">说明</span><span class="sxs-lookup"><span data-stu-id="df111-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="df111-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="df111-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="df111-114">流</span><span class="sxs-lookup"><span data-stu-id="df111-114">Stream</span></span>          | [<span data-ttu-id="df111-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="df111-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="df111-116">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="df111-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="df111-117">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="df111-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="df111-118">流</span><span class="sxs-lookup"><span data-stu-id="df111-118">Stream</span></span>          | [<span data-ttu-id="df111-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="df111-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="df111-120">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="df111-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="df111-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="df111-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="df111-122">Stream</span><span class="sxs-lookup"><span data-stu-id="df111-122">Stream</span></span>          | [<span data-ttu-id="df111-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="df111-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="df111-124">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="df111-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="df111-125">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="df111-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="df111-126">Stream</span><span class="sxs-lookup"><span data-stu-id="df111-126">Stream</span></span>          | [<span data-ttu-id="df111-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="df111-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="df111-128">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="df111-128">Get the count of unique users by Outlook desktop version.</span></span> |
