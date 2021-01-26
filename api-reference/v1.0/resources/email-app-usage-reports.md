---
title: 电子邮件应用使用情况报表
description: 电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: df0b0bcea7631551ff0dc75162b9d294a7760f99
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981669"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="9e383-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="9e383-104">Email app usage reports</span></span>

<span data-ttu-id="9e383-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e383-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e383-106">电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。</span><span class="sxs-lookup"><span data-stu-id="9e383-106">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="9e383-107">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="9e383-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="9e383-108">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报告 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="9e383-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="9e383-109">报告</span><span class="sxs-lookup"><span data-stu-id="9e383-109">Reports</span></span>

| <span data-ttu-id="9e383-110">函数</span><span class="sxs-lookup"><span data-stu-id="9e383-110">Function</span></span>                                 | <span data-ttu-id="9e383-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e383-111">Return Type</span></span> | <span data-ttu-id="9e383-112">说明</span><span class="sxs-lookup"><span data-stu-id="9e383-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="9e383-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="9e383-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="9e383-114">Stream</span><span class="sxs-lookup"><span data-stu-id="9e383-114">Stream</span></span>      | <span data-ttu-id="9e383-115">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9e383-115">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="9e383-116">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="9e383-116">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="9e383-117">Stream</span><span class="sxs-lookup"><span data-stu-id="9e383-117">Stream</span></span>      | <span data-ttu-id="9e383-118">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="9e383-118">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="9e383-119">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="9e383-119">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="9e383-120">Stream</span><span class="sxs-lookup"><span data-stu-id="9e383-120">Stream</span></span>      | <span data-ttu-id="9e383-121">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="9e383-121">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="9e383-122">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="9e383-122">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="9e383-123">Stream</span><span class="sxs-lookup"><span data-stu-id="9e383-123">Stream</span></span>      | <span data-ttu-id="9e383-124">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="9e383-124">Get the count of unique users by Outlook desktop version.</span></span> |

