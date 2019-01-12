---
title: OneDrive 活动报表
description: OneDrive 活动报表可用于获取每个有权使用 OneDrive 的用户的活动，具体是以用户与 OneDrive 文件的交互为依据。 此类报表也有助于了解以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a493114fb44ddd9040675c9feb6a3b21ce543009
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923073"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="28bda-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="28bda-104">OneDrive activity reports</span></span>

<span data-ttu-id="28bda-105">OneDrive 活动报表可用于获取每个有权使用 OneDrive 的用户的活动，具体是以用户与 OneDrive 文件的交互为依据。</span><span class="sxs-lookup"><span data-stu-id="28bda-105">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="28bda-106">此类报表也有助于了解以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="28bda-106">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="28bda-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="28bda-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="28bda-108">报表</span><span class="sxs-lookup"><span data-stu-id="28bda-108">Reports</span></span>

| <span data-ttu-id="28bda-109">函数</span><span class="sxs-lookup"><span data-stu-id="28bda-109">Function</span></span>                                 | <span data-ttu-id="28bda-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="28bda-110">Return Type</span></span> | <span data-ttu-id="28bda-111">说明</span><span class="sxs-lookup"><span data-stu-id="28bda-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="28bda-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="28bda-112">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="28bda-113">Stream</span><span class="sxs-lookup"><span data-stu-id="28bda-113">Stream</span></span>      | <span data-ttu-id="28bda-114">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="28bda-114">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="28bda-115">获取用户数</span><span class="sxs-lookup"><span data-stu-id="28bda-115">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="28bda-116">Stream</span><span class="sxs-lookup"><span data-stu-id="28bda-116">Stream</span></span>      | <span data-ttu-id="28bda-117">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="28bda-117">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="28bda-118">获取文件数</span><span class="sxs-lookup"><span data-stu-id="28bda-118">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="28bda-119">Stream</span><span class="sxs-lookup"><span data-stu-id="28bda-119">Stream</span></span>      | <span data-ttu-id="28bda-120">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="28bda-120">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

