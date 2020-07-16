---
title: 电子邮件应用使用情况报表
description: 您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f666fed390272002f2e556f355618fddc935981e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896901"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="6c799-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="6c799-104">Email app usage reports</span></span>

<span data-ttu-id="6c799-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c799-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c799-106">您可以查看使用多少个电子邮件应用程序连接到 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="6c799-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="6c799-107">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="6c799-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="6c799-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-电子邮件应用程序使用](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="6c799-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="6c799-109">报表</span><span class="sxs-lookup"><span data-stu-id="6c799-109">Reports</span></span>

| <span data-ttu-id="6c799-110">函数</span><span class="sxs-lookup"><span data-stu-id="6c799-110">Function</span></span>                                 | <span data-ttu-id="6c799-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="6c799-111">CSV return type</span></span> | <span data-ttu-id="6c799-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="6c799-112">JSON return type</span></span>                         | <span data-ttu-id="6c799-113">说明</span><span class="sxs-lookup"><span data-stu-id="6c799-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6c799-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="6c799-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="6c799-115">Stream</span><span class="sxs-lookup"><span data-stu-id="6c799-115">Stream</span></span>          | [<span data-ttu-id="6c799-116">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="6c799-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="6c799-117">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6c799-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="6c799-118">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="6c799-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="6c799-119">Stream</span><span class="sxs-lookup"><span data-stu-id="6c799-119">Stream</span></span>          | [<span data-ttu-id="6c799-120">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="6c799-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="6c799-121">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="6c799-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="6c799-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="6c799-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="6c799-123">Stream</span><span class="sxs-lookup"><span data-stu-id="6c799-123">Stream</span></span>          | [<span data-ttu-id="6c799-124">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="6c799-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="6c799-125">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="6c799-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="6c799-126">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="6c799-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="6c799-127">Stream</span><span class="sxs-lookup"><span data-stu-id="6c799-127">Stream</span></span>          | [<span data-ttu-id="6c799-128">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="6c799-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="6c799-129">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="6c799-129">Get the count of unique users by Outlook desktop version.</span></span> |
