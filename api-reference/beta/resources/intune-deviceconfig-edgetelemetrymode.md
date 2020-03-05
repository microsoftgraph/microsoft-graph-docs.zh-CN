---
title: edgeTelemetryMode 枚举类型
description: 发送到 Microsoft 365 analytics 的浏览数据的类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 09cd5012d0b3a07a203b89ed76062232c47cfa82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530035"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="451be-103">edgeTelemetryMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="451be-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="451be-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="451be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="451be-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="451be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="451be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="451be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="451be-107">发送到 Microsoft 365 analytics 的浏览数据的类型</span><span class="sxs-lookup"><span data-stu-id="451be-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="451be-108">成员</span><span class="sxs-lookup"><span data-stu-id="451be-108">Members</span></span>
|<span data-ttu-id="451be-109">成员</span><span class="sxs-lookup"><span data-stu-id="451be-109">Member</span></span>|<span data-ttu-id="451be-110">值</span><span class="sxs-lookup"><span data-stu-id="451be-110">Value</span></span>|<span data-ttu-id="451be-111">说明</span><span class="sxs-lookup"><span data-stu-id="451be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="451be-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="451be-112">notConfigured</span></span>|<span data-ttu-id="451be-113">0</span><span class="sxs-lookup"><span data-stu-id="451be-113">0</span></span>|<span data-ttu-id="451be-114">默认值–没有收集或发送的遥测数据</span><span class="sxs-lookup"><span data-stu-id="451be-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="451be-115">在内</span><span class="sxs-lookup"><span data-stu-id="451be-115">intranet</span></span>|<span data-ttu-id="451be-116">1 </span><span class="sxs-lookup"><span data-stu-id="451be-116">1</span></span>|<span data-ttu-id="451be-117">仅允许发送 intranet 历史记录：仅发送 intranet 网站的浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="451be-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="451be-118">访问</span><span class="sxs-lookup"><span data-stu-id="451be-118">internet</span></span>|<span data-ttu-id="451be-119">2 </span><span class="sxs-lookup"><span data-stu-id="451be-119">2</span></span>|<span data-ttu-id="451be-120">仅允许发送 internet 历史记录：仅发送 internet 网站的浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="451be-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="451be-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="451be-121">intranetAndInternet</span></span>|<span data-ttu-id="451be-122">3 </span><span class="sxs-lookup"><span data-stu-id="451be-122">3</span></span>|<span data-ttu-id="451be-123">允许同时发送 intranet 和 internet 历史记录：为 intranet 和 internet 站点发送浏览历史记录数据</span><span class="sxs-lookup"><span data-stu-id="451be-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



