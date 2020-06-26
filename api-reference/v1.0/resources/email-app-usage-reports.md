---
title: 电子邮件应用使用情况报表
description: 电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: d34a829063ca5c5f5be6ad6b8bf822b8a2cd8520
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898266"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="681e4-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="681e4-104">Email app usage reports</span></span>

<span data-ttu-id="681e4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="681e4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="681e4-106">电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。</span><span class="sxs-lookup"><span data-stu-id="681e4-106">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="681e4-107">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="681e4-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="681e4-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-电子邮件应用程序使用](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="681e4-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="681e4-109">报表</span><span class="sxs-lookup"><span data-stu-id="681e4-109">Reports</span></span>

| <span data-ttu-id="681e4-110">函数</span><span class="sxs-lookup"><span data-stu-id="681e4-110">Function</span></span>                                 | <span data-ttu-id="681e4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="681e4-111">Return Type</span></span> | <span data-ttu-id="681e4-112">说明</span><span class="sxs-lookup"><span data-stu-id="681e4-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="681e4-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="681e4-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="681e4-114">Stream</span><span class="sxs-lookup"><span data-stu-id="681e4-114">Stream</span></span>      | <span data-ttu-id="681e4-115">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="681e4-115">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="681e4-116">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="681e4-116">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="681e4-117">Stream</span><span class="sxs-lookup"><span data-stu-id="681e4-117">Stream</span></span>      | <span data-ttu-id="681e4-118">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="681e4-118">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="681e4-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="681e4-119">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="681e4-120">Stream</span><span class="sxs-lookup"><span data-stu-id="681e4-120">Stream</span></span>      | <span data-ttu-id="681e4-121">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="681e4-121">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="681e4-122">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="681e4-122">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="681e4-123">Stream</span><span class="sxs-lookup"><span data-stu-id="681e4-123">Stream</span></span>      | <span data-ttu-id="681e4-124">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="681e4-124">Get the count of unique users by Outlook desktop version.</span></span> |
