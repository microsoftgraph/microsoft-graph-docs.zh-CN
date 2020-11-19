---
title: win32LobAppPowerShellScriptRuleOperationType 枚举类型
description: 包含所有受支持的 Powershell 脚本输出检测类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5f49038bd4896a273442aad17324a122e44fc2d0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284587"
---
# <a name="win32lobapppowershellscriptruleoperationtype-enum-type"></a><span data-ttu-id="64f96-103">win32LobAppPowerShellScriptRuleOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="64f96-103">win32LobAppPowerShellScriptRuleOperationType enum type</span></span>

<span data-ttu-id="64f96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64f96-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64f96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f96-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64f96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f96-107">包含所有受支持的 Powershell 脚本输出检测类型。</span><span class="sxs-lookup"><span data-stu-id="64f96-107">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="64f96-108">成员</span><span class="sxs-lookup"><span data-stu-id="64f96-108">Members</span></span>
|<span data-ttu-id="64f96-109">成员</span><span class="sxs-lookup"><span data-stu-id="64f96-109">Member</span></span>|<span data-ttu-id="64f96-110">值</span><span class="sxs-lookup"><span data-stu-id="64f96-110">Value</span></span>|<span data-ttu-id="64f96-111">Description</span><span class="sxs-lookup"><span data-stu-id="64f96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f96-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="64f96-112">notConfigured</span></span>|<span data-ttu-id="64f96-113">0</span><span class="sxs-lookup"><span data-stu-id="64f96-113">0</span></span>|<span data-ttu-id="64f96-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="64f96-114">Not configured.</span></span>|
|<span data-ttu-id="64f96-115">字符串</span><span class="sxs-lookup"><span data-stu-id="64f96-115">string</span></span>|<span data-ttu-id="64f96-116">1</span><span class="sxs-lookup"><span data-stu-id="64f96-116">1</span></span>|<span data-ttu-id="64f96-117">输出数据类型为 string。</span><span class="sxs-lookup"><span data-stu-id="64f96-117">Output data type is string.</span></span>|
|<span data-ttu-id="64f96-118">dateTime</span><span class="sxs-lookup"><span data-stu-id="64f96-118">dateTime</span></span>|<span data-ttu-id="64f96-119">双面</span><span class="sxs-lookup"><span data-stu-id="64f96-119">2</span></span>|<span data-ttu-id="64f96-120">输出数据类型为 "日期时间"。</span><span class="sxs-lookup"><span data-stu-id="64f96-120">Output data type is date time.</span></span>|
|<span data-ttu-id="64f96-121">integer</span><span class="sxs-lookup"><span data-stu-id="64f96-121">integer</span></span>|<span data-ttu-id="64f96-122">第三章</span><span class="sxs-lookup"><span data-stu-id="64f96-122">3</span></span>|<span data-ttu-id="64f96-123">输出数据类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="64f96-123">Output data type is integer.</span></span>|
|<span data-ttu-id="64f96-124">float</span><span class="sxs-lookup"><span data-stu-id="64f96-124">float</span></span>|<span data-ttu-id="64f96-125">4 </span><span class="sxs-lookup"><span data-stu-id="64f96-125">4</span></span>|<span data-ttu-id="64f96-126">输出数据类型为 float。</span><span class="sxs-lookup"><span data-stu-id="64f96-126">Output data type is float.</span></span>|
|<span data-ttu-id="64f96-127">version</span><span class="sxs-lookup"><span data-stu-id="64f96-127">version</span></span>|<span data-ttu-id="64f96-128">5 </span><span class="sxs-lookup"><span data-stu-id="64f96-128">5</span></span>|<span data-ttu-id="64f96-129">输出数据类型为版本。</span><span class="sxs-lookup"><span data-stu-id="64f96-129">Output data type is version.</span></span>|
|<span data-ttu-id="64f96-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="64f96-130">boolean</span></span>|<span data-ttu-id="64f96-131">6 </span><span class="sxs-lookup"><span data-stu-id="64f96-131">6</span></span>|<span data-ttu-id="64f96-132">输出数据类型为布尔值。</span><span class="sxs-lookup"><span data-stu-id="64f96-132">Output data type is boolean.</span></span>|




