---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 57dcba3a91b15b4980d9e76b7aad6251008f5966
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555289"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="b6c78-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="b6c78-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c78-105">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="b6c78-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="b6c78-106">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="b6c78-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="b6c78-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="b6c78-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="b6c78-108">报表</span><span class="sxs-lookup"><span data-stu-id="b6c78-108">Reports</span></span>

| <span data-ttu-id="b6c78-109">函数</span><span class="sxs-lookup"><span data-stu-id="b6c78-109">Function</span></span>                                 | <span data-ttu-id="b6c78-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="b6c78-110">CSV return type</span></span> | <span data-ttu-id="b6c78-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="b6c78-111">JSON return type</span></span>                         | <span data-ttu-id="b6c78-112">说明</span><span class="sxs-lookup"><span data-stu-id="b6c78-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b6c78-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="b6c78-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="b6c78-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b6c78-114">Stream</span></span>          | [<span data-ttu-id="b6c78-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="b6c78-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="b6c78-116">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b6c78-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="b6c78-117">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="b6c78-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="b6c78-118">Stream</span><span class="sxs-lookup"><span data-stu-id="b6c78-118">Stream</span></span>          | [<span data-ttu-id="b6c78-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="b6c78-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="b6c78-120">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="b6c78-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="b6c78-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="b6c78-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="b6c78-122">Stream</span><span class="sxs-lookup"><span data-stu-id="b6c78-122">Stream</span></span>          | [<span data-ttu-id="b6c78-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b6c78-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="b6c78-124">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="b6c78-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
