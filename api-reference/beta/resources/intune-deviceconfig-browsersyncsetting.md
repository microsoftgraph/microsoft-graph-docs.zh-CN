---
title: browserSyncSetting 枚举类型
description: 允许未配置 () 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。 选项可阻止跨设备同步，但允许用户重写。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6495134df04ac1b94df605b866862273a5321bc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016378"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="e918b-104">browserSyncSetting 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e918b-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="e918b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e918b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e918b-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e918b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e918b-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e918b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e918b-108">允许未配置 () 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。</span><span class="sxs-lookup"><span data-stu-id="e918b-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="e918b-109">选项可阻止跨设备同步，但允许用户重写。</span><span class="sxs-lookup"><span data-stu-id="e918b-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="e918b-110">成员</span><span class="sxs-lookup"><span data-stu-id="e918b-110">Members</span></span>
|<span data-ttu-id="e918b-111">成员</span><span class="sxs-lookup"><span data-stu-id="e918b-111">Member</span></span>|<span data-ttu-id="e918b-112">值</span><span class="sxs-lookup"><span data-stu-id="e918b-112">Value</span></span>|<span data-ttu-id="e918b-113">说明</span><span class="sxs-lookup"><span data-stu-id="e918b-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e918b-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e918b-114">notConfigured</span></span>|<span data-ttu-id="e918b-115">0</span><span class="sxs-lookup"><span data-stu-id="e918b-115">0</span></span>|<span data-ttu-id="e918b-116">默认值–允许跨设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="e918b-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="e918b-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="e918b-117">blockedWithUserOverride</span></span>|<span data-ttu-id="e918b-118">1 </span><span class="sxs-lookup"><span data-stu-id="e918b-118">1</span></span>|<span data-ttu-id="e918b-119">阻止跨用户设备同步浏览器设置，允许用户重写设置。</span><span class="sxs-lookup"><span data-stu-id="e918b-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="e918b-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="e918b-120">blocked</span></span>|<span data-ttu-id="e918b-121">2 </span><span class="sxs-lookup"><span data-stu-id="e918b-121">2</span></span>|<span data-ttu-id="e918b-122">绝对阻止跨用户设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="e918b-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|






