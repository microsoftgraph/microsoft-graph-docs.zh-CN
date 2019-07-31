---
title: OneDrive 活动报表
description: 您可以通过查看其与 OneDrive 上的文件的交互, 获取获得使用 OneDrive 的每个用户的活动。 它还可帮助您了解通过显示共享文件数而进行的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 710b2ed88deeec26846bb5afe7503808d8c470c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009438"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="e20d3-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="e20d3-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e20d3-105">您可以通过查看其与 OneDrive 上的文件的交互, 获取获得使用 OneDrive 的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="e20d3-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="e20d3-106">它还可帮助您了解通过显示共享文件数而进行的协作级别。</span><span class="sxs-lookup"><span data-stu-id="e20d3-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="e20d3-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="e20d3-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="e20d3-108">报表</span><span class="sxs-lookup"><span data-stu-id="e20d3-108">Reports</span></span>

| <span data-ttu-id="e20d3-109">函数</span><span class="sxs-lookup"><span data-stu-id="e20d3-109">Function</span></span>                                 | <span data-ttu-id="e20d3-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="e20d3-110">CSV return type</span></span> | <span data-ttu-id="e20d3-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="e20d3-111">JSON return type</span></span>                         | <span data-ttu-id="e20d3-112">说明</span><span class="sxs-lookup"><span data-stu-id="e20d3-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e20d3-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="e20d3-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="e20d3-114">流</span><span class="sxs-lookup"><span data-stu-id="e20d3-114">Stream</span></span>          | [<span data-ttu-id="e20d3-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e20d3-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="e20d3-116">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e20d3-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="e20d3-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e20d3-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="e20d3-118">Stream</span><span class="sxs-lookup"><span data-stu-id="e20d3-118">Stream</span></span>          | [<span data-ttu-id="e20d3-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e20d3-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="e20d3-120">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="e20d3-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="e20d3-121">获取文件数</span><span class="sxs-lookup"><span data-stu-id="e20d3-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="e20d3-122">Stream</span><span class="sxs-lookup"><span data-stu-id="e20d3-122">Stream</span></span>          | [<span data-ttu-id="e20d3-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e20d3-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="e20d3-124">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="e20d3-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
