---
title: win32LobAppPowerShellScriptDetectionType 枚举类型
description: 包含所有受支持的 Powershell 脚本输出检测类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 517863d85f06a65346a5e40a6eef321566c8db77
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694058"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a><span data-ttu-id="9ac53-103">win32LobAppPowerShellScriptDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9ac53-103">win32LobAppPowerShellScriptDetectionType enum type</span></span>

<span data-ttu-id="9ac53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ac53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ac53-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ac53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ac53-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ac53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac53-107">包含所有受支持的 Powershell 脚本输出检测类型。</span><span class="sxs-lookup"><span data-stu-id="9ac53-107">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="9ac53-108">成员</span><span class="sxs-lookup"><span data-stu-id="9ac53-108">Members</span></span>
|<span data-ttu-id="9ac53-109">成员</span><span class="sxs-lookup"><span data-stu-id="9ac53-109">Member</span></span>|<span data-ttu-id="9ac53-110">值</span><span class="sxs-lookup"><span data-stu-id="9ac53-110">Value</span></span>|<span data-ttu-id="9ac53-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ac53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac53-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9ac53-112">notConfigured</span></span>|<span data-ttu-id="9ac53-113">0</span><span class="sxs-lookup"><span data-stu-id="9ac53-113">0</span></span>|<span data-ttu-id="9ac53-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="9ac53-114">Not configured.</span></span>|
|<span data-ttu-id="9ac53-115">string</span><span class="sxs-lookup"><span data-stu-id="9ac53-115">string</span></span>|<span data-ttu-id="9ac53-116">1</span><span class="sxs-lookup"><span data-stu-id="9ac53-116">1</span></span>|<span data-ttu-id="9ac53-117">输出数据类型为 string。</span><span class="sxs-lookup"><span data-stu-id="9ac53-117">Output data type is string.</span></span>|
|<span data-ttu-id="9ac53-118">dateTime</span><span class="sxs-lookup"><span data-stu-id="9ac53-118">dateTime</span></span>|<span data-ttu-id="9ac53-119">双面</span><span class="sxs-lookup"><span data-stu-id="9ac53-119">2</span></span>|<span data-ttu-id="9ac53-120">输出数据类型为 "日期时间"。</span><span class="sxs-lookup"><span data-stu-id="9ac53-120">Output data type is date time.</span></span>|
|<span data-ttu-id="9ac53-121">integer</span><span class="sxs-lookup"><span data-stu-id="9ac53-121">integer</span></span>|<span data-ttu-id="9ac53-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9ac53-122">3</span></span>|<span data-ttu-id="9ac53-123">输出数据类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="9ac53-123">Output data type is integer.</span></span>|
|<span data-ttu-id="9ac53-124">float</span><span class="sxs-lookup"><span data-stu-id="9ac53-124">float</span></span>|<span data-ttu-id="9ac53-125">4 </span><span class="sxs-lookup"><span data-stu-id="9ac53-125">4</span></span>|<span data-ttu-id="9ac53-126">输出数据类型为 float。</span><span class="sxs-lookup"><span data-stu-id="9ac53-126">Output data type is float.</span></span>|
|<span data-ttu-id="9ac53-127">version</span><span class="sxs-lookup"><span data-stu-id="9ac53-127">version</span></span>|<span data-ttu-id="9ac53-128">5 </span><span class="sxs-lookup"><span data-stu-id="9ac53-128">5</span></span>|<span data-ttu-id="9ac53-129">输出数据类型为版本。</span><span class="sxs-lookup"><span data-stu-id="9ac53-129">Output data type is version.</span></span>|
|<span data-ttu-id="9ac53-130">boolean</span><span class="sxs-lookup"><span data-stu-id="9ac53-130">boolean</span></span>|<span data-ttu-id="9ac53-131">6 </span><span class="sxs-lookup"><span data-stu-id="9ac53-131">6</span></span>|<span data-ttu-id="9ac53-132">输出数据类型为布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ac53-132">Output data type is boolean.</span></span>|





