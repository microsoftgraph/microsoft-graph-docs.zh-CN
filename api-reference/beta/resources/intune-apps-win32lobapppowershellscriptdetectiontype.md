---
title: win32LobAppPowerShellScriptDetectionType 枚举类型
description: 包含所有受支持的 Powershell 脚本输出检测类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cbadfc4ccf93db91478752335eaa59dac4a3eee0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490572"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a><span data-ttu-id="adf05-103">win32LobAppPowerShellScriptDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="adf05-103">win32LobAppPowerShellScriptDetectionType enum type</span></span>

<span data-ttu-id="adf05-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="adf05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adf05-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="adf05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adf05-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="adf05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adf05-107">包含所有受支持的 Powershell 脚本输出检测类型。</span><span class="sxs-lookup"><span data-stu-id="adf05-107">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="adf05-108">成员</span><span class="sxs-lookup"><span data-stu-id="adf05-108">Members</span></span>
|<span data-ttu-id="adf05-109">成员</span><span class="sxs-lookup"><span data-stu-id="adf05-109">Member</span></span>|<span data-ttu-id="adf05-110">值</span><span class="sxs-lookup"><span data-stu-id="adf05-110">Value</span></span>|<span data-ttu-id="adf05-111">说明</span><span class="sxs-lookup"><span data-stu-id="adf05-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adf05-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="adf05-112">notConfigured</span></span>|<span data-ttu-id="adf05-113">0</span><span class="sxs-lookup"><span data-stu-id="adf05-113">0</span></span>|<span data-ttu-id="adf05-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="adf05-114">Not configured.</span></span>|
|<span data-ttu-id="adf05-115">string</span><span class="sxs-lookup"><span data-stu-id="adf05-115">string</span></span>|<span data-ttu-id="adf05-116">1 </span><span class="sxs-lookup"><span data-stu-id="adf05-116">1</span></span>|<span data-ttu-id="adf05-117">输出数据类型为 string。</span><span class="sxs-lookup"><span data-stu-id="adf05-117">Output data type is string.</span></span>|
|<span data-ttu-id="adf05-118">dateTime</span><span class="sxs-lookup"><span data-stu-id="adf05-118">dateTime</span></span>|<span data-ttu-id="adf05-119">2 </span><span class="sxs-lookup"><span data-stu-id="adf05-119">2</span></span>|<span data-ttu-id="adf05-120">输出数据类型为 "日期时间"。</span><span class="sxs-lookup"><span data-stu-id="adf05-120">Output data type is date time.</span></span>|
|<span data-ttu-id="adf05-121">integer</span><span class="sxs-lookup"><span data-stu-id="adf05-121">integer</span></span>|<span data-ttu-id="adf05-122">3 </span><span class="sxs-lookup"><span data-stu-id="adf05-122">3</span></span>|<span data-ttu-id="adf05-123">输出数据类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="adf05-123">Output data type is integer.</span></span>|
|<span data-ttu-id="adf05-124">点数</span><span class="sxs-lookup"><span data-stu-id="adf05-124">float</span></span>|<span data-ttu-id="adf05-125">4 </span><span class="sxs-lookup"><span data-stu-id="adf05-125">4</span></span>|<span data-ttu-id="adf05-126">输出数据类型为 float。</span><span class="sxs-lookup"><span data-stu-id="adf05-126">Output data type is float.</span></span>|
|<span data-ttu-id="adf05-127">version</span><span class="sxs-lookup"><span data-stu-id="adf05-127">version</span></span>|<span data-ttu-id="adf05-128">5 </span><span class="sxs-lookup"><span data-stu-id="adf05-128">5</span></span>|<span data-ttu-id="adf05-129">输出数据类型为版本。</span><span class="sxs-lookup"><span data-stu-id="adf05-129">Output data type is version.</span></span>|
|<span data-ttu-id="adf05-130">boolean</span><span class="sxs-lookup"><span data-stu-id="adf05-130">boolean</span></span>|<span data-ttu-id="adf05-131">6 </span><span class="sxs-lookup"><span data-stu-id="adf05-131">6</span></span>|<span data-ttu-id="adf05-132">输出数据类型为布尔值。</span><span class="sxs-lookup"><span data-stu-id="adf05-132">Output data type is boolean.</span></span>|



