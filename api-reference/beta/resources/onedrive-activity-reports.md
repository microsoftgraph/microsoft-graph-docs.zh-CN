---
title: OneDrive 活动报表
description: 您可以通过查看其与 onedrive 上的文件的交互, 获取获得使用 onedrive 的每个用户的活动。 它还可帮助您了解通过显示共享文件数而进行的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3a99ba5dbc1a61b11d916c9fff90cec53a4eeaf9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345521"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="67819-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="67819-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67819-105">您可以通过查看其与 onedrive 上的文件的交互, 获取获得使用 onedrive 的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="67819-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="67819-106">它还可帮助您了解通过显示共享文件数而进行的协作级别。</span><span class="sxs-lookup"><span data-stu-id="67819-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="67819-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="67819-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="67819-108">报表</span><span class="sxs-lookup"><span data-stu-id="67819-108">Reports</span></span>

| <span data-ttu-id="67819-109">函数</span><span class="sxs-lookup"><span data-stu-id="67819-109">Function</span></span>                                 | <span data-ttu-id="67819-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="67819-110">CSV return type</span></span> | <span data-ttu-id="67819-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="67819-111">JSON return type</span></span>                         | <span data-ttu-id="67819-112">说明</span><span class="sxs-lookup"><span data-stu-id="67819-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="67819-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="67819-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="67819-114">Stream</span><span class="sxs-lookup"><span data-stu-id="67819-114">Stream</span></span>          | [<span data-ttu-id="67819-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="67819-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="67819-116">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="67819-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="67819-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="67819-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="67819-118">Stream</span><span class="sxs-lookup"><span data-stu-id="67819-118">Stream</span></span>          | [<span data-ttu-id="67819-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="67819-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="67819-120">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="67819-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="67819-121">获取文件数</span><span class="sxs-lookup"><span data-stu-id="67819-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="67819-122">Stream</span><span class="sxs-lookup"><span data-stu-id="67819-122">Stream</span></span>          | [<span data-ttu-id="67819-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="67819-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="67819-124">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="67819-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
