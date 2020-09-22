---
title: OneDrive 活动报表
description: 您可以通过查看其与 OneDrive 上的文件的交互，获取获得使用 OneDrive 的每个用户的活动。 它还可帮助您了解通过显示共享文件数而进行的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 656d722a9d63e460cd4b62e87a0b2fd8483e37c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092333"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="e27a5-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="e27a5-104">OneDrive activity reports</span></span>

<span data-ttu-id="e27a5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e27a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e27a5-106">您可以通过查看其与 OneDrive 上的文件的交互，获取获得使用 OneDrive 的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="e27a5-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="e27a5-107">它还可帮助您了解通过显示共享文件数而进行的协作级别。</span><span class="sxs-lookup"><span data-stu-id="e27a5-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="e27a5-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 reports-OneDrive For business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="e27a5-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="e27a5-109">报表</span><span class="sxs-lookup"><span data-stu-id="e27a5-109">Reports</span></span>

| <span data-ttu-id="e27a5-110">函数</span><span class="sxs-lookup"><span data-stu-id="e27a5-110">Function</span></span>                                 | <span data-ttu-id="e27a5-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="e27a5-111">CSV return type</span></span> | <span data-ttu-id="e27a5-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="e27a5-112">JSON return type</span></span>                         | <span data-ttu-id="e27a5-113">说明</span><span class="sxs-lookup"><span data-stu-id="e27a5-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e27a5-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="e27a5-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="e27a5-115">Stream</span><span class="sxs-lookup"><span data-stu-id="e27a5-115">Stream</span></span>          | [<span data-ttu-id="e27a5-116">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e27a5-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="e27a5-117">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e27a5-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="e27a5-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e27a5-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="e27a5-119">Stream</span><span class="sxs-lookup"><span data-stu-id="e27a5-119">Stream</span></span>          | [<span data-ttu-id="e27a5-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e27a5-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="e27a5-121">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="e27a5-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="e27a5-122">获取文件数</span><span class="sxs-lookup"><span data-stu-id="e27a5-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="e27a5-123">Stream</span><span class="sxs-lookup"><span data-stu-id="e27a5-123">Stream</span></span>          | [<span data-ttu-id="e27a5-124">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e27a5-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="e27a5-125">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="e27a5-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |


