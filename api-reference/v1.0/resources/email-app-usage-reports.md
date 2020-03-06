---
title: 电子邮件应用使用情况报表
description: 电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 9ea3418dd065758fb2d623c9995b78126ea3d475
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532987"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="2ad0a-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="2ad0a-104">Email app usage reports</span></span>

<span data-ttu-id="2ad0a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ad0a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ad0a-106">电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-106">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="2ad0a-107">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="2ad0a-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="2ad0a-109">报表</span><span class="sxs-lookup"><span data-stu-id="2ad0a-109">Reports</span></span>

| <span data-ttu-id="2ad0a-110">函数</span><span class="sxs-lookup"><span data-stu-id="2ad0a-110">Function</span></span>                                 | <span data-ttu-id="2ad0a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ad0a-111">Return Type</span></span> | <span data-ttu-id="2ad0a-112">说明</span><span class="sxs-lookup"><span data-stu-id="2ad0a-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="2ad0a-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="2ad0a-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="2ad0a-114">Stream</span><span class="sxs-lookup"><span data-stu-id="2ad0a-114">Stream</span></span>      | <span data-ttu-id="2ad0a-115">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-115">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="2ad0a-116">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="2ad0a-116">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="2ad0a-117">Stream</span><span class="sxs-lookup"><span data-stu-id="2ad0a-117">Stream</span></span>      | <span data-ttu-id="2ad0a-118">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-118">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="2ad0a-119">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="2ad0a-119">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="2ad0a-120">Stream</span><span class="sxs-lookup"><span data-stu-id="2ad0a-120">Stream</span></span>      | <span data-ttu-id="2ad0a-121">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-121">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="2ad0a-122">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="2ad0a-122">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="2ad0a-123">Stream</span><span class="sxs-lookup"><span data-stu-id="2ad0a-123">Stream</span></span>      | <span data-ttu-id="2ad0a-124">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="2ad0a-124">Get the count of unique users by Outlook desktop version.</span></span> |
