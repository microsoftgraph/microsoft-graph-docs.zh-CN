---
title: edgeTelemetryMode 枚举类型
description: 发送到 Microsoft 365 analytics 的浏览数据的类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 87663359f015d2b0ae854715b4ed7fe09a7c1973
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728575"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="6ff02-103">edgeTelemetryMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6ff02-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="6ff02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ff02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ff02-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ff02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff02-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ff02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff02-107">发送到 Microsoft 365 analytics 的浏览数据的类型</span><span class="sxs-lookup"><span data-stu-id="6ff02-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="6ff02-108">成员</span><span class="sxs-lookup"><span data-stu-id="6ff02-108">Members</span></span>
|<span data-ttu-id="6ff02-109">成员</span><span class="sxs-lookup"><span data-stu-id="6ff02-109">Member</span></span>|<span data-ttu-id="6ff02-110">值</span><span class="sxs-lookup"><span data-stu-id="6ff02-110">Value</span></span>|<span data-ttu-id="6ff02-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ff02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff02-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6ff02-112">notConfigured</span></span>|<span data-ttu-id="6ff02-113">0</span><span class="sxs-lookup"><span data-stu-id="6ff02-113">0</span></span>|<span data-ttu-id="6ff02-114">默认值–没有收集或发送的遥测数据</span><span class="sxs-lookup"><span data-stu-id="6ff02-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="6ff02-115">在内</span><span class="sxs-lookup"><span data-stu-id="6ff02-115">intranet</span></span>|<span data-ttu-id="6ff02-116">1</span><span class="sxs-lookup"><span data-stu-id="6ff02-116">1</span></span>|<span data-ttu-id="6ff02-117">仅允许发送 intranet 历史记录：仅发送 intranet 网站的浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="6ff02-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="6ff02-118">访问</span><span class="sxs-lookup"><span data-stu-id="6ff02-118">internet</span></span>|<span data-ttu-id="6ff02-119">双面</span><span class="sxs-lookup"><span data-stu-id="6ff02-119">2</span></span>|<span data-ttu-id="6ff02-120">仅允许发送 internet 历史记录：仅发送 internet 网站的浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="6ff02-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="6ff02-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="6ff02-121">intranetAndInternet</span></span>|<span data-ttu-id="6ff02-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6ff02-122">3</span></span>|<span data-ttu-id="6ff02-123">允许同时发送 intranet 和 internet 历史记录：为 intranet 和 internet 站点发送浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="6ff02-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





