---
title: 电子邮件应用使用情况报表
description: 电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
ms.openlocfilehash: 87f04af05aeb55758ec2bdb01fa4f909c7ffa788
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007960"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="90881-104">电子邮件应用使用情况报表</span><span class="sxs-lookup"><span data-stu-id="90881-104">Email app usage reports</span></span>

<span data-ttu-id="90881-105">电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。</span><span class="sxs-lookup"><span data-stu-id="90881-105">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="90881-106">此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。</span><span class="sxs-lookup"><span data-stu-id="90881-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="90881-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="90881-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="90881-108">报表</span><span class="sxs-lookup"><span data-stu-id="90881-108">Reports</span></span>

| <span data-ttu-id="90881-109">函数</span><span class="sxs-lookup"><span data-stu-id="90881-109">Function</span></span>                                 | <span data-ttu-id="90881-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="90881-110">Return Type</span></span> | <span data-ttu-id="90881-111">说明</span><span class="sxs-lookup"><span data-stu-id="90881-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="90881-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="90881-112">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="90881-113">Stream</span><span class="sxs-lookup"><span data-stu-id="90881-113">Stream</span></span>      | <span data-ttu-id="90881-114">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="90881-114">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="90881-115">获取应用用户数</span><span class="sxs-lookup"><span data-stu-id="90881-115">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="90881-116">Stream</span><span class="sxs-lookup"><span data-stu-id="90881-116">Stream</span></span>      | <span data-ttu-id="90881-117">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="90881-117">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="90881-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="90881-118">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="90881-119">Stream</span><span class="sxs-lookup"><span data-stu-id="90881-119">Stream</span></span>      | <span data-ttu-id="90881-120">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="90881-120">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="90881-121">获取版本用户数</span><span class="sxs-lookup"><span data-stu-id="90881-121">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="90881-122">Stream</span><span class="sxs-lookup"><span data-stu-id="90881-122">Stream</span></span>      | <span data-ttu-id="90881-123">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="90881-123">Get the count of unique users by Outlook desktop version.</span></span> |
