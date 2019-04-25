---
title: Skype for Business 对等活动报表
description: 你可以在组织中获取对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8802430e6f2725b520e7b558f48ed760c26b7588
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579021"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="f6237-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="f6237-104">Skype for Business peer-to-peer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6237-105">你可以在组织中获取对等活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f6237-105">You can get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="f6237-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="f6237-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="f6237-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="f6237-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="f6237-108">报表</span><span class="sxs-lookup"><span data-stu-id="f6237-108">Reports</span></span>

| <span data-ttu-id="f6237-109">函数</span><span class="sxs-lookup"><span data-stu-id="f6237-109">Function</span></span>                                 | <span data-ttu-id="f6237-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="f6237-110">CSV return type</span></span> | <span data-ttu-id="f6237-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="f6237-111">JSON return type</span></span>                         | <span data-ttu-id="f6237-112">说明</span><span class="sxs-lookup"><span data-stu-id="f6237-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f6237-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="f6237-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="f6237-114">Stream</span><span class="sxs-lookup"><span data-stu-id="f6237-114">Stream</span></span>          | [<span data-ttu-id="f6237-115">skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f6237-115">skypeForBusinessPeerToPeerActivityCounts</span></span>](../resources/skypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="f6237-116">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="f6237-116">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="f6237-117">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="f6237-117">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="f6237-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="f6237-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="f6237-119">Stream</span><span class="sxs-lookup"><span data-stu-id="f6237-119">Stream</span></span>          | [<span data-ttu-id="f6237-120">skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f6237-120">skypeForBusinessPeerToPeerActivityUserCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="f6237-121">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="f6237-121">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="f6237-122">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="f6237-122">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="f6237-123">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="f6237-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="f6237-124">Stream</span><span class="sxs-lookup"><span data-stu-id="f6237-124">Stream</span></span>          | [<span data-ttu-id="f6237-125">skypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="f6237-125">skypeForBusinessPeerToPeerActivityMinuteCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="f6237-126">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="f6237-126">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="f6237-127">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="f6237-127">Types of sessions include audio and video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-peer-to-peer-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
