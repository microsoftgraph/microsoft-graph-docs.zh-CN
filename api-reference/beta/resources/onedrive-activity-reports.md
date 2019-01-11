---
title: OneDrive 活动报表
description: 您可以获取许可使用 OneDrive 看它们与 OneDrive 上的文件的交互的每个用户的活动。 此外可帮助您了解协作事通过显示共享的文件数的级别。
localization_priority: Normal
ms.openlocfilehash: fc87eebeb7c0df1bd6d08a82fa67ccd6d9fa40a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814488"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="8a4a2-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="8a4a2-104">OneDrive activity reports</span></span>

> <span data-ttu-id="8a4a2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a4a2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a4a2-107">您可以获取许可使用 OneDrive 看它们与 OneDrive 上的文件的交互的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-107">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="8a4a2-108">此外可帮助您了解协作事通过显示共享的文件数的级别。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-108">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="8a4a2-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="8a4a2-110">报表</span><span class="sxs-lookup"><span data-stu-id="8a4a2-110">Reports</span></span>

| <span data-ttu-id="8a4a2-111">函数</span><span class="sxs-lookup"><span data-stu-id="8a4a2-111">Function</span></span>                                 | <span data-ttu-id="8a4a2-112">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="8a4a2-112">CSV return type</span></span> | <span data-ttu-id="8a4a2-113">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="8a4a2-113">JSON return type</span></span>                         | <span data-ttu-id="8a4a2-114">说明</span><span class="sxs-lookup"><span data-stu-id="8a4a2-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="8a4a2-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="8a4a2-115">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="8a4a2-116">Stream</span><span class="sxs-lookup"><span data-stu-id="8a4a2-116">Stream</span></span>          | [<span data-ttu-id="8a4a2-117">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8a4a2-117">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="8a4a2-118">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-118">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="8a4a2-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="8a4a2-119">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="8a4a2-120">Stream</span><span class="sxs-lookup"><span data-stu-id="8a4a2-120">Stream</span></span>          | [<span data-ttu-id="8a4a2-121">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8a4a2-121">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="8a4a2-122">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-122">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="8a4a2-123">获取文件数</span><span class="sxs-lookup"><span data-stu-id="8a4a2-123">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="8a4a2-124">Stream</span><span class="sxs-lookup"><span data-stu-id="8a4a2-124">Stream</span></span>          | [<span data-ttu-id="8a4a2-125">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8a4a2-125">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="8a4a2-126">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="8a4a2-126">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
