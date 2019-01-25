---
title: 电子邮件应用使用情况报表
description: 您可以看到多少电子邮件应用程序用于连接到 Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: 92390033e544bc0163923e2bdad6e99212b66f92
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527778"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="ddeb9-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="ddeb9-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddeb9-105">您可以看到多少电子邮件应用程序用于连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="ddeb9-106">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="ddeb9-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="ddeb9-108">报表</span><span class="sxs-lookup"><span data-stu-id="ddeb9-108">Reports</span></span>

| <span data-ttu-id="ddeb9-109">函数</span><span class="sxs-lookup"><span data-stu-id="ddeb9-109">Function</span></span>                                 | <span data-ttu-id="ddeb9-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="ddeb9-110">CSV return type</span></span> | <span data-ttu-id="ddeb9-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="ddeb9-111">JSON return type</span></span>                         | <span data-ttu-id="ddeb9-112">说明</span><span class="sxs-lookup"><span data-stu-id="ddeb9-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ddeb9-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="ddeb9-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="ddeb9-114">Stream</span><span class="sxs-lookup"><span data-stu-id="ddeb9-114">Stream</span></span>          | [<span data-ttu-id="ddeb9-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ddeb9-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="ddeb9-116">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="ddeb9-117">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="ddeb9-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="ddeb9-118">Stream</span><span class="sxs-lookup"><span data-stu-id="ddeb9-118">Stream</span></span>          | [<span data-ttu-id="ddeb9-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="ddeb9-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="ddeb9-120">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="ddeb9-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="ddeb9-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="ddeb9-122">Stream</span><span class="sxs-lookup"><span data-stu-id="ddeb9-122">Stream</span></span>          | [<span data-ttu-id="ddeb9-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ddeb9-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="ddeb9-124">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="ddeb9-125">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="ddeb9-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="ddeb9-126">Stream</span><span class="sxs-lookup"><span data-stu-id="ddeb9-126">Stream</span></span>          | [<span data-ttu-id="ddeb9-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="ddeb9-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="ddeb9-128">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="ddeb9-128">Get the count of unique users by Outlook desktop version.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
