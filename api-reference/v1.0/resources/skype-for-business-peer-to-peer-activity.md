---
title: Skype for Business 对等活动报表
description: Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
ms.openlocfilehash: 08021570e70847bf230997b991e5901f887d0e4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009496"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="ffbd5-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="ffbd5-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="ffbd5-105">Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-105">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="ffbd5-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="ffbd5-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="ffbd5-108">报表</span><span class="sxs-lookup"><span data-stu-id="ffbd5-108">Reports</span></span>

| <span data-ttu-id="ffbd5-109">函数</span><span class="sxs-lookup"><span data-stu-id="ffbd5-109">Function</span></span>                                 | <span data-ttu-id="ffbd5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffbd5-110">Return Type</span></span> | <span data-ttu-id="ffbd5-111">说明</span><span class="sxs-lookup"><span data-stu-id="ffbd5-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="ffbd5-112">获取活动数</span><span class="sxs-lookup"><span data-stu-id="ffbd5-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="ffbd5-113">Stream</span><span class="sxs-lookup"><span data-stu-id="ffbd5-113">Stream</span></span>      | <span data-ttu-id="ffbd5-114">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-114">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="ffbd5-115">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-115">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="ffbd5-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="ffbd5-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="ffbd5-117">Stream</span><span class="sxs-lookup"><span data-stu-id="ffbd5-117">Stream</span></span>      | <span data-ttu-id="ffbd5-118">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-118">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="ffbd5-119">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-119">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="ffbd5-120">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="ffbd5-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="ffbd5-121">Stream</span><span class="sxs-lookup"><span data-stu-id="ffbd5-121">Stream</span></span>      | <span data-ttu-id="ffbd5-122">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-122">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="ffbd5-123">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="ffbd5-123">Types of sessions include audio and video.</span></span> |

