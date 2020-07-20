---
title: win32LobAppRegistryRuleOperationType 枚举类型
description: 包含所有受支持的注册表数据检测类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b0aefbf5fd234bac0704c9c9f983e19ed11cbcfe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790304"
---
# <a name="win32lobappregistryruleoperationtype-enum-type"></a><span data-ttu-id="77591-103">win32LobAppRegistryRuleOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="77591-103">win32LobAppRegistryRuleOperationType enum type</span></span>

<span data-ttu-id="77591-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77591-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77591-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77591-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77591-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77591-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77591-107">包含所有受支持的注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="77591-107">Contains all supported registry data detection type.</span></span>

## <a name="members"></a><span data-ttu-id="77591-108">成员</span><span class="sxs-lookup"><span data-stu-id="77591-108">Members</span></span>
|<span data-ttu-id="77591-109">成员</span><span class="sxs-lookup"><span data-stu-id="77591-109">Member</span></span>|<span data-ttu-id="77591-110">值</span><span class="sxs-lookup"><span data-stu-id="77591-110">Value</span></span>|<span data-ttu-id="77591-111">说明</span><span class="sxs-lookup"><span data-stu-id="77591-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77591-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="77591-112">notConfigured</span></span>|<span data-ttu-id="77591-113">0</span><span class="sxs-lookup"><span data-stu-id="77591-113">0</span></span>|<span data-ttu-id="77591-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="77591-114">Not configured.</span></span>|
|<span data-ttu-id="77591-115">存在</span><span class="sxs-lookup"><span data-stu-id="77591-115">exists</span></span>|<span data-ttu-id="77591-116">1 </span><span class="sxs-lookup"><span data-stu-id="77591-116">1</span></span>|<span data-ttu-id="77591-117">指定的注册表项或值存在。</span><span class="sxs-lookup"><span data-stu-id="77591-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="77591-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="77591-118">doesNotExist</span></span>|<span data-ttu-id="77591-119">双面</span><span class="sxs-lookup"><span data-stu-id="77591-119">2</span></span>|<span data-ttu-id="77591-120">指定的注册表项或值不存在。</span><span class="sxs-lookup"><span data-stu-id="77591-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="77591-121">string</span><span class="sxs-lookup"><span data-stu-id="77591-121">string</span></span>|<span data-ttu-id="77591-122">第三章</span><span class="sxs-lookup"><span data-stu-id="77591-122">3</span></span>|<span data-ttu-id="77591-123">字符串值类型。</span><span class="sxs-lookup"><span data-stu-id="77591-123">String value type.</span></span>|
|<span data-ttu-id="77591-124">integer</span><span class="sxs-lookup"><span data-stu-id="77591-124">integer</span></span>|<span data-ttu-id="77591-125">4 </span><span class="sxs-lookup"><span data-stu-id="77591-125">4</span></span>|<span data-ttu-id="77591-126">整型值类型。</span><span class="sxs-lookup"><span data-stu-id="77591-126">Integer value type.</span></span>|
|<span data-ttu-id="77591-127">version</span><span class="sxs-lookup"><span data-stu-id="77591-127">version</span></span>|<span data-ttu-id="77591-128">5 </span><span class="sxs-lookup"><span data-stu-id="77591-128">5</span></span>|<span data-ttu-id="77591-129">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="77591-129">Version value type.</span></span>|



