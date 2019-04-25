---
title: Yammer 活动报表
description: 您可以通过在组织中生成多少活动以及在 yammer 上进行 post (如和阅读邮件) 的唯一用户的数量来了解您的组织对 yammer 的服务级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d5953d8bd53158b2ec0532deb47c48028ba1b8c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523796"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="8293b-103">Yammer 活动报表</span><span class="sxs-lookup"><span data-stu-id="8293b-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8293b-104">您可以通过在组织中生成多少活动以及在 yammer 上进行 post (如和阅读邮件) 的唯一用户的数量来了解您的组织对 yammer 的服务级别。</span><span class="sxs-lookup"><span data-stu-id="8293b-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="8293b-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="8293b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="8293b-106">报表</span><span class="sxs-lookup"><span data-stu-id="8293b-106">Reports</span></span>

| <span data-ttu-id="8293b-107">函数</span><span class="sxs-lookup"><span data-stu-id="8293b-107">Function</span></span>                                 | <span data-ttu-id="8293b-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="8293b-108">CSV return type</span></span> | <span data-ttu-id="8293b-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="8293b-109">JSON return type</span></span>                         | <span data-ttu-id="8293b-110">说明</span><span class="sxs-lookup"><span data-stu-id="8293b-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="8293b-111">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="8293b-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="8293b-112">Stream</span><span class="sxs-lookup"><span data-stu-id="8293b-112">Stream</span></span>          | [<span data-ttu-id="8293b-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8293b-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="8293b-114">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8293b-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="8293b-115">获取活动数</span><span class="sxs-lookup"><span data-stu-id="8293b-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="8293b-116">Stream</span><span class="sxs-lookup"><span data-stu-id="8293b-116">Stream</span></span>          | [<span data-ttu-id="8293b-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8293b-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="8293b-118">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="8293b-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="8293b-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="8293b-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="8293b-120">Stream</span><span class="sxs-lookup"><span data-stu-id="8293b-120">Stream</span></span>          | [<span data-ttu-id="8293b-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8293b-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="8293b-122">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="8293b-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
