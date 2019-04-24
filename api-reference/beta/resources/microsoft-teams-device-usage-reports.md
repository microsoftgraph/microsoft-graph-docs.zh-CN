---
title: Microsoft Teams 设备使用情况报告
description: '使用 microsoft 团队设备使用情况报告可深入了解组织中的 microsoft 团队设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d19df5132a67ac5862535a329eadbdff7044798c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457107"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="ed05e-103">Microsoft Teams 设备使用情况报告</span><span class="sxs-lookup"><span data-stu-id="ed05e-103">Microsoft Teams device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed05e-104">使用 microsoft 团队设备使用情况报告可深入了解组织中的 microsoft 团队设备使用情况。</span><span class="sxs-lookup"><span data-stu-id="ed05e-104">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="ed05e-105">方法</span><span class="sxs-lookup"><span data-stu-id="ed05e-105">Methods</span></span>

| <span data-ttu-id="ed05e-106">方法</span><span class="sxs-lookup"><span data-stu-id="ed05e-106">Method</span></span>                                   | <span data-ttu-id="ed05e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed05e-107">Return Type</span></span>                              | <span data-ttu-id="ed05e-108">说明</span><span class="sxs-lookup"><span data-stu-id="ed05e-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="ed05e-109">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="ed05e-109">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="ed05e-110">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ed05e-110">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="ed05e-111">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ed05e-111">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="ed05e-112">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="ed05e-112">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="ed05e-113">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ed05e-113">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="ed05e-114">按设备类型获取每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="ed05e-114">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="ed05e-115">获取分发用户计数</span><span class="sxs-lookup"><span data-stu-id="ed05e-115">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="ed05e-116">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ed05e-116">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="ed05e-117">在选定的时间段内按设备类型获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="ed05e-117">Get the number of unique users by device type over the selected time period.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
