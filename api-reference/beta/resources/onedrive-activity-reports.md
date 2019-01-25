---
title: OneDrive 活动报表
description: 您可以获取许可使用 OneDrive 看它们与 OneDrive 上的文件的交互的每个用户的活动。 此外可帮助您了解协作事通过显示共享的文件数的级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9075bd042a0c27debc8017a007351428191e9d43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519225"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="dd369-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="dd369-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd369-105">您可以获取许可使用 OneDrive 看它们与 OneDrive 上的文件的交互的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="dd369-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="dd369-106">此外可帮助您了解协作事通过显示共享的文件数的级别。</span><span class="sxs-lookup"><span data-stu-id="dd369-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="dd369-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="dd369-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="dd369-108">报表</span><span class="sxs-lookup"><span data-stu-id="dd369-108">Reports</span></span>

| <span data-ttu-id="dd369-109">函数</span><span class="sxs-lookup"><span data-stu-id="dd369-109">Function</span></span>                                 | <span data-ttu-id="dd369-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="dd369-110">CSV return type</span></span> | <span data-ttu-id="dd369-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="dd369-111">JSON return type</span></span>                         | <span data-ttu-id="dd369-112">说明</span><span class="sxs-lookup"><span data-stu-id="dd369-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="dd369-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="dd369-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="dd369-114">Stream</span><span class="sxs-lookup"><span data-stu-id="dd369-114">Stream</span></span>          | [<span data-ttu-id="dd369-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="dd369-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="dd369-116">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dd369-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="dd369-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="dd369-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="dd369-118">Stream</span><span class="sxs-lookup"><span data-stu-id="dd369-118">Stream</span></span>          | [<span data-ttu-id="dd369-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="dd369-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="dd369-120">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="dd369-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="dd369-121">获取文件数</span><span class="sxs-lookup"><span data-stu-id="dd369-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="dd369-122">Stream</span><span class="sxs-lookup"><span data-stu-id="dd369-122">Stream</span></span>          | [<span data-ttu-id="dd369-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="dd369-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="dd369-124">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="dd369-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
