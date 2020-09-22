---
title: win32LobAppPowerShellScriptRuleOperationType 枚举类型
description: 包含所有受支持的 Powershell 脚本输出检测类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 00eda4f735b9cdcdc177d8a7db9a1c74ad253f9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092830"
---
# <a name="win32lobapppowershellscriptruleoperationtype-enum-type"></a><span data-ttu-id="a1739-103">win32LobAppPowerShellScriptRuleOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a1739-103">win32LobAppPowerShellScriptRuleOperationType enum type</span></span>

<span data-ttu-id="a1739-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1739-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1739-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1739-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1739-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1739-107">包含所有受支持的 Powershell 脚本输出检测类型。</span><span class="sxs-lookup"><span data-stu-id="a1739-107">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="a1739-108">成员</span><span class="sxs-lookup"><span data-stu-id="a1739-108">Members</span></span>
|<span data-ttu-id="a1739-109">成员</span><span class="sxs-lookup"><span data-stu-id="a1739-109">Member</span></span>|<span data-ttu-id="a1739-110">值</span><span class="sxs-lookup"><span data-stu-id="a1739-110">Value</span></span>|<span data-ttu-id="a1739-111">说明</span><span class="sxs-lookup"><span data-stu-id="a1739-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1739-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a1739-112">notConfigured</span></span>|<span data-ttu-id="a1739-113">0</span><span class="sxs-lookup"><span data-stu-id="a1739-113">0</span></span>|<span data-ttu-id="a1739-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="a1739-114">Not configured.</span></span>|
|<span data-ttu-id="a1739-115">string</span><span class="sxs-lookup"><span data-stu-id="a1739-115">string</span></span>|<span data-ttu-id="a1739-116">1 </span><span class="sxs-lookup"><span data-stu-id="a1739-116">1</span></span>|<span data-ttu-id="a1739-117">输出数据类型为 string。</span><span class="sxs-lookup"><span data-stu-id="a1739-117">Output data type is string.</span></span>|
|<span data-ttu-id="a1739-118">dateTime</span><span class="sxs-lookup"><span data-stu-id="a1739-118">dateTime</span></span>|<span data-ttu-id="a1739-119">2 </span><span class="sxs-lookup"><span data-stu-id="a1739-119">2</span></span>|<span data-ttu-id="a1739-120">输出数据类型为 "日期时间"。</span><span class="sxs-lookup"><span data-stu-id="a1739-120">Output data type is date time.</span></span>|
|<span data-ttu-id="a1739-121">integer</span><span class="sxs-lookup"><span data-stu-id="a1739-121">integer</span></span>|<span data-ttu-id="a1739-122">第三章</span><span class="sxs-lookup"><span data-stu-id="a1739-122">3</span></span>|<span data-ttu-id="a1739-123">输出数据类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="a1739-123">Output data type is integer.</span></span>|
|<span data-ttu-id="a1739-124">点数</span><span class="sxs-lookup"><span data-stu-id="a1739-124">float</span></span>|<span data-ttu-id="a1739-125">4 </span><span class="sxs-lookup"><span data-stu-id="a1739-125">4</span></span>|<span data-ttu-id="a1739-126">输出数据类型为 float。</span><span class="sxs-lookup"><span data-stu-id="a1739-126">Output data type is float.</span></span>|
|<span data-ttu-id="a1739-127">version</span><span class="sxs-lookup"><span data-stu-id="a1739-127">version</span></span>|<span data-ttu-id="a1739-128">5 </span><span class="sxs-lookup"><span data-stu-id="a1739-128">5</span></span>|<span data-ttu-id="a1739-129">输出数据类型为版本。</span><span class="sxs-lookup"><span data-stu-id="a1739-129">Output data type is version.</span></span>|
|<span data-ttu-id="a1739-130">boolean</span><span class="sxs-lookup"><span data-stu-id="a1739-130">boolean</span></span>|<span data-ttu-id="a1739-131">6 </span><span class="sxs-lookup"><span data-stu-id="a1739-131">6</span></span>|<span data-ttu-id="a1739-132">输出数据类型为布尔值。</span><span class="sxs-lookup"><span data-stu-id="a1739-132">Output data type is boolean.</span></span>|






