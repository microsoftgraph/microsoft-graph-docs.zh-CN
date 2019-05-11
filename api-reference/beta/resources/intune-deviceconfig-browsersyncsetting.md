---
title: browserSyncSetting 枚举类型
description: 允许 (未配置) 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。 选项可阻止跨设备同步, 但允许用户重写。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33b7edf861154005b2548441dcf3cc776451f3ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947468"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="b2b50-104">browserSyncSetting 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b2b50-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="b2b50-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2b50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2b50-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2b50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2b50-107">允许 (未配置) 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。</span><span class="sxs-lookup"><span data-stu-id="b2b50-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="b2b50-108">选项可阻止跨设备同步, 但允许用户重写。</span><span class="sxs-lookup"><span data-stu-id="b2b50-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="b2b50-109">成员</span><span class="sxs-lookup"><span data-stu-id="b2b50-109">Members</span></span>
|<span data-ttu-id="b2b50-110">成员</span><span class="sxs-lookup"><span data-stu-id="b2b50-110">Member</span></span>|<span data-ttu-id="b2b50-111">值</span><span class="sxs-lookup"><span data-stu-id="b2b50-111">Value</span></span>|<span data-ttu-id="b2b50-112">说明</span><span class="sxs-lookup"><span data-stu-id="b2b50-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2b50-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b2b50-113">notConfigured</span></span>|<span data-ttu-id="b2b50-114">0</span><span class="sxs-lookup"><span data-stu-id="b2b50-114">0</span></span>|<span data-ttu-id="b2b50-115">默认值–允许跨设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="b2b50-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="b2b50-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="b2b50-116">blockedWithUserOverride</span></span>|<span data-ttu-id="b2b50-117">1</span><span class="sxs-lookup"><span data-stu-id="b2b50-117">1</span></span>|<span data-ttu-id="b2b50-118">阻止跨用户设备同步浏览器设置, 允许用户重写设置。</span><span class="sxs-lookup"><span data-stu-id="b2b50-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="b2b50-119">堵塞</span><span class="sxs-lookup"><span data-stu-id="b2b50-119">blocked</span></span>|<span data-ttu-id="b2b50-120">双面</span><span class="sxs-lookup"><span data-stu-id="b2b50-120">2</span></span>|<span data-ttu-id="b2b50-121">绝对阻止跨用户设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="b2b50-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|




