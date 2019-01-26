---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d19df5132a67ac5862535a329eadbdff7044798c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576638"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="d4681-103">Microsoft Teams 设备使用情况报告</span><span class="sxs-lookup"><span data-stu-id="d4681-103">Microsoft Teams device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4681-104">使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。</span><span class="sxs-lookup"><span data-stu-id="d4681-104">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="d4681-105">方法</span><span class="sxs-lookup"><span data-stu-id="d4681-105">Methods</span></span>

| <span data-ttu-id="d4681-106">方法</span><span class="sxs-lookup"><span data-stu-id="d4681-106">Method</span></span>                                   | <span data-ttu-id="d4681-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4681-107">Return Type</span></span>                              | <span data-ttu-id="d4681-108">说明</span><span class="sxs-lookup"><span data-stu-id="d4681-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="d4681-109">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="d4681-109">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="d4681-110">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="d4681-110">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="d4681-111">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d4681-111">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="d4681-112">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="d4681-112">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="d4681-113">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d4681-113">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="d4681-114">按设备类型获取每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="d4681-114">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="d4681-115">获取分发用户计数</span><span class="sxs-lookup"><span data-stu-id="d4681-115">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="d4681-116">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d4681-116">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="d4681-117">在选定的时间段内按设备类型获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="d4681-117">Get the number of unique users by device type over the selected time period.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
