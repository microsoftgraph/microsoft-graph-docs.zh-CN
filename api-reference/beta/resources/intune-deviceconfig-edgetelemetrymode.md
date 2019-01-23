---
title: edgeTelemetryMode 枚举类型
description: 浏览数据发送到 Microsoft 365 分析的类型
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429444"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="07b04-103">edgeTelemetryMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="07b04-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="07b04-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="07b04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07b04-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="07b04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07b04-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07b04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07b04-107">浏览数据发送到 Microsoft 365 分析的类型</span><span class="sxs-lookup"><span data-stu-id="07b04-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="07b04-108">成员</span><span class="sxs-lookup"><span data-stu-id="07b04-108">Members</span></span>
|<span data-ttu-id="07b04-109">成员</span><span class="sxs-lookup"><span data-stu-id="07b04-109">Member</span></span>|<span data-ttu-id="07b04-110">值</span><span class="sxs-lookup"><span data-stu-id="07b04-110">Value</span></span>|<span data-ttu-id="07b04-111">说明</span><span class="sxs-lookup"><span data-stu-id="07b04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07b04-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="07b04-112">notConfigured</span></span>|<span data-ttu-id="07b04-113">0</span><span class="sxs-lookup"><span data-stu-id="07b04-113">0</span></span>|<span data-ttu-id="07b04-114">默认值 – 没有遥测数据收集或发送</span><span class="sxs-lookup"><span data-stu-id="07b04-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="07b04-115">intranet</span><span class="sxs-lookup"><span data-stu-id="07b04-115">intranet</span></span>|<span data-ttu-id="07b04-116">1</span><span class="sxs-lookup"><span data-stu-id="07b04-116">1</span></span>|<span data-ttu-id="07b04-117">允许发送 intranet 历史记录： 仅发送浏览 intranet 网站的历史记录数据</span><span class="sxs-lookup"><span data-stu-id="07b04-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="07b04-118">internet</span><span class="sxs-lookup"><span data-stu-id="07b04-118">internet</span></span>|<span data-ttu-id="07b04-119">2</span><span class="sxs-lookup"><span data-stu-id="07b04-119">2</span></span>|<span data-ttu-id="07b04-120">允许发送 internet 历史记录： 仅发送浏览的 internet 站点的历史记录数据</span><span class="sxs-lookup"><span data-stu-id="07b04-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="07b04-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="07b04-121">intranetAndInternet</span></span>|<span data-ttu-id="07b04-122">3</span><span class="sxs-lookup"><span data-stu-id="07b04-122">3</span></span>|<span data-ttu-id="07b04-123">允许发送 intranet 和 internet 历史记录： 发送浏览 intranet 和 internet 网站的历史记录数据</span><span class="sxs-lookup"><span data-stu-id="07b04-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




