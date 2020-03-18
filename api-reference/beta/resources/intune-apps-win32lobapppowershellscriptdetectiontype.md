---
title: win32LobAppPowerShellScriptDetectionType 枚举类型
description: 包含所有受支持的 Powershell 脚本输出检测类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 47fcba9cd87a128c45f79685073d9c5740c8ea0e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797603"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a><span data-ttu-id="f75c6-103">win32LobAppPowerShellScriptDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f75c6-103">win32LobAppPowerShellScriptDetectionType enum type</span></span>

> <span data-ttu-id="f75c6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f75c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f75c6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f75c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f75c6-106">包含所有受支持的 Powershell 脚本输出检测类型。</span><span class="sxs-lookup"><span data-stu-id="f75c6-106">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="f75c6-107">成员</span><span class="sxs-lookup"><span data-stu-id="f75c6-107">Members</span></span>
|<span data-ttu-id="f75c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="f75c6-108">Member</span></span>|<span data-ttu-id="f75c6-109">值</span><span class="sxs-lookup"><span data-stu-id="f75c6-109">Value</span></span>|<span data-ttu-id="f75c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="f75c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f75c6-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f75c6-111">notConfigured</span></span>|<span data-ttu-id="f75c6-112">0</span><span class="sxs-lookup"><span data-stu-id="f75c6-112">0</span></span>|<span data-ttu-id="f75c6-113">未配置。</span><span class="sxs-lookup"><span data-stu-id="f75c6-113">Not configured.</span></span>|
|<span data-ttu-id="f75c6-114">string</span><span class="sxs-lookup"><span data-stu-id="f75c6-114">string</span></span>|<span data-ttu-id="f75c6-115">1</span><span class="sxs-lookup"><span data-stu-id="f75c6-115">1</span></span>|<span data-ttu-id="f75c6-116">输出数据类型为 string。</span><span class="sxs-lookup"><span data-stu-id="f75c6-116">Output data type is string.</span></span>|
|<span data-ttu-id="f75c6-117">dateTime</span><span class="sxs-lookup"><span data-stu-id="f75c6-117">dateTime</span></span>|<span data-ttu-id="f75c6-118">双面</span><span class="sxs-lookup"><span data-stu-id="f75c6-118">2</span></span>|<span data-ttu-id="f75c6-119">输出数据类型为 "日期时间"。</span><span class="sxs-lookup"><span data-stu-id="f75c6-119">Output data type is date time.</span></span>|
|<span data-ttu-id="f75c6-120">integer</span><span class="sxs-lookup"><span data-stu-id="f75c6-120">integer</span></span>|<span data-ttu-id="f75c6-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f75c6-121">3</span></span>|<span data-ttu-id="f75c6-122">输出数据类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="f75c6-122">Output data type is integer.</span></span>|
|<span data-ttu-id="f75c6-123">点数</span><span class="sxs-lookup"><span data-stu-id="f75c6-123">float</span></span>|<span data-ttu-id="f75c6-124">4 </span><span class="sxs-lookup"><span data-stu-id="f75c6-124">4</span></span>|<span data-ttu-id="f75c6-125">输出数据类型为 float。</span><span class="sxs-lookup"><span data-stu-id="f75c6-125">Output data type is float.</span></span>|
|<span data-ttu-id="f75c6-126">version</span><span class="sxs-lookup"><span data-stu-id="f75c6-126">version</span></span>|<span data-ttu-id="f75c6-127">5 </span><span class="sxs-lookup"><span data-stu-id="f75c6-127">5</span></span>|<span data-ttu-id="f75c6-128">输出数据类型为版本。</span><span class="sxs-lookup"><span data-stu-id="f75c6-128">Output data type is version.</span></span>|
|<span data-ttu-id="f75c6-129">boolean</span><span class="sxs-lookup"><span data-stu-id="f75c6-129">boolean</span></span>|<span data-ttu-id="f75c6-130">6 </span><span class="sxs-lookup"><span data-stu-id="f75c6-130">6</span></span>|<span data-ttu-id="f75c6-131">输出数据类型为布尔值。</span><span class="sxs-lookup"><span data-stu-id="f75c6-131">Output data type is boolean.</span></span>|



