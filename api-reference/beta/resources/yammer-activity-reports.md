---
title: Yammer 活动报表
description: 您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509936"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="fd8d7-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="fd8d7-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd8d7-104">您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。</span><span class="sxs-lookup"><span data-stu-id="fd8d7-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="fd8d7-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="fd8d7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="fd8d7-106">报表</span><span class="sxs-lookup"><span data-stu-id="fd8d7-106">Reports</span></span>

| <span data-ttu-id="fd8d7-107">函数</span><span class="sxs-lookup"><span data-stu-id="fd8d7-107">Function</span></span>                                 | <span data-ttu-id="fd8d7-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="fd8d7-108">CSV return type</span></span> | <span data-ttu-id="fd8d7-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="fd8d7-109">JSON return type</span></span>                         | <span data-ttu-id="fd8d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="fd8d7-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="fd8d7-111">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="fd8d7-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="fd8d7-112">Stream</span><span class="sxs-lookup"><span data-stu-id="fd8d7-112">Stream</span></span>          | [<span data-ttu-id="fd8d7-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fd8d7-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="fd8d7-114">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fd8d7-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="fd8d7-115">获取活动数</span><span class="sxs-lookup"><span data-stu-id="fd8d7-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="fd8d7-116">Stream</span><span class="sxs-lookup"><span data-stu-id="fd8d7-116">Stream</span></span>          | [<span data-ttu-id="fd8d7-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="fd8d7-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="fd8d7-118">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="fd8d7-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="fd8d7-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="fd8d7-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="fd8d7-120">Stream</span><span class="sxs-lookup"><span data-stu-id="fd8d7-120">Stream</span></span>          | [<span data-ttu-id="fd8d7-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="fd8d7-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="fd8d7-122">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="fd8d7-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
