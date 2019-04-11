---
title: edgeTelemetryMode 枚举类型
description: 发送到 Microsoft 365 analytics 的浏览数据的类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d671849e34d27403450ae6324b824a92ae9d9b4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774587"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="3befb-103">edgeTelemetryMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3befb-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="3befb-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3befb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3befb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3befb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3befb-106">发送到 Microsoft 365 analytics 的浏览数据的类型</span><span class="sxs-lookup"><span data-stu-id="3befb-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="3befb-107">成员</span><span class="sxs-lookup"><span data-stu-id="3befb-107">Members</span></span>
|<span data-ttu-id="3befb-108">成员</span><span class="sxs-lookup"><span data-stu-id="3befb-108">Member</span></span>|<span data-ttu-id="3befb-109">值</span><span class="sxs-lookup"><span data-stu-id="3befb-109">Value</span></span>|<span data-ttu-id="3befb-110">说明</span><span class="sxs-lookup"><span data-stu-id="3befb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3befb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3befb-111">notConfigured</span></span>|<span data-ttu-id="3befb-112">0</span><span class="sxs-lookup"><span data-stu-id="3befb-112">0</span></span>|<span data-ttu-id="3befb-113">默认值–没有收集或发送的遥测数据</span><span class="sxs-lookup"><span data-stu-id="3befb-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="3befb-114">在内</span><span class="sxs-lookup"><span data-stu-id="3befb-114">intranet</span></span>|<span data-ttu-id="3befb-115">1</span><span class="sxs-lookup"><span data-stu-id="3befb-115">1</span></span>|<span data-ttu-id="3befb-116">仅允许发送 intranet 历史记录: 仅发送 intranet 网站的浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="3befb-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="3befb-117">访问</span><span class="sxs-lookup"><span data-stu-id="3befb-117">internet</span></span>|<span data-ttu-id="3befb-118">双面</span><span class="sxs-lookup"><span data-stu-id="3befb-118">2</span></span>|<span data-ttu-id="3befb-119">仅允许发送 internet 历史记录: 仅发送 internet 网站的浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="3befb-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="3befb-120">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="3befb-120">intranetAndInternet</span></span>|<span data-ttu-id="3befb-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3befb-121">3</span></span>|<span data-ttu-id="3befb-122">允许同时发送 intranet 和 internet 历史记录: 为 intranet 和 internet 站点发送浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="3befb-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





