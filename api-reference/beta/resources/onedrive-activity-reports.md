---
title: OneDrive 活动报表
description: 通过查看每个许可使用 OneDrive 的用户与 OneDrive 上的文件的交互，你可以获取他们的活动。 它还通过显示共享文件的数量来帮助你了解进行协作的级别。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d0c069d2787b30f37e634757127b6141843a9ed
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983599"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="9a14a-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="9a14a-104">OneDrive activity reports</span></span>

<span data-ttu-id="9a14a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a14a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a14a-106">通过查看每个许可使用 OneDrive 的用户与 OneDrive 上的文件的交互，你可以获取他们的活动。</span><span class="sxs-lookup"><span data-stu-id="9a14a-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="9a14a-107">它还通过显示共享文件的数量来帮助你了解进行协作的级别。</span><span class="sxs-lookup"><span data-stu-id="9a14a-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="9a14a-108">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="9a14a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="9a14a-109">报告</span><span class="sxs-lookup"><span data-stu-id="9a14a-109">Reports</span></span>

| <span data-ttu-id="9a14a-110">函数</span><span class="sxs-lookup"><span data-stu-id="9a14a-110">Function</span></span>                                 | <span data-ttu-id="9a14a-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="9a14a-111">CSV return type</span></span> | <span data-ttu-id="9a14a-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="9a14a-112">JSON return type</span></span>                         | <span data-ttu-id="9a14a-113">说明</span><span class="sxs-lookup"><span data-stu-id="9a14a-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="9a14a-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="9a14a-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="9a14a-115">Stream</span><span class="sxs-lookup"><span data-stu-id="9a14a-115">Stream</span></span>          | [<span data-ttu-id="9a14a-116">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9a14a-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="9a14a-117">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9a14a-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="9a14a-118">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="9a14a-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="9a14a-119">Stream</span><span class="sxs-lookup"><span data-stu-id="9a14a-119">Stream</span></span>          | [<span data-ttu-id="9a14a-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="9a14a-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="9a14a-121">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="9a14a-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="9a14a-122">获取文件数</span><span class="sxs-lookup"><span data-stu-id="9a14a-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="9a14a-123">Stream</span><span class="sxs-lookup"><span data-stu-id="9a14a-123">Stream</span></span>          | [<span data-ttu-id="9a14a-124">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="9a14a-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="9a14a-125">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="9a14a-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |


