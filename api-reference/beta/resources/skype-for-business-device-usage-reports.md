---
title: Skype for Business 设备使用情况报表
description: 您可以获取有关在组织中使用的客户端和设备的类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b55017967bd28337f5015791864e81d274f99681
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554875"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="5e1d3-104">Skype for Business 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="5e1d3-104">Skype for Business device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e1d3-105">您可以获取有关在组织中使用的客户端和设备的类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-105">You can get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="5e1d3-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="5e1d3-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="5e1d3-108">报表</span><span class="sxs-lookup"><span data-stu-id="5e1d3-108">Reports</span></span>

| <span data-ttu-id="5e1d3-109">函数</span><span class="sxs-lookup"><span data-stu-id="5e1d3-109">Function</span></span>                                 | <span data-ttu-id="5e1d3-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="5e1d3-110">CSV return type</span></span> | <span data-ttu-id="5e1d3-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="5e1d3-111">JSON return type</span></span>                         | <span data-ttu-id="5e1d3-112">说明</span><span class="sxs-lookup"><span data-stu-id="5e1d3-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5e1d3-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="5e1d3-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="5e1d3-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5e1d3-114">Stream</span></span>          | [<span data-ttu-id="5e1d3-115">skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5e1d3-115">skypeForBusinessDeviceUsageUserDetail</span></span>](../resources/skypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="5e1d3-116">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-116">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="5e1d3-117">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="5e1d3-117">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="5e1d3-118">Stream</span><span class="sxs-lookup"><span data-stu-id="5e1d3-118">Stream</span></span>          | [<span data-ttu-id="5e1d3-119">skypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="5e1d3-119">skypeForBusinessDeviceUsageDistributionUserCounts</span></span>](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="5e1d3-120">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-120">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="5e1d3-121">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-121">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="5e1d3-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="5e1d3-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="5e1d3-123">Stream</span><span class="sxs-lookup"><span data-stu-id="5e1d3-123">Stream</span></span>          | [<span data-ttu-id="5e1d3-124">skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="5e1d3-124">skypeForBusinessDeviceUsageUserCounts</span></span>](../resources/skypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="5e1d3-125">获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-125">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="5e1d3-126">还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。</span><span class="sxs-lookup"><span data-stu-id="5e1d3-126">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
