---
title: browserSyncSetting 枚举类型
description: 允许 (未配置) 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。 选项可阻止跨设备同步, 但允许用户重写。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71b5fd7addebdb24fce07644da9b33a2bb41f936
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152168"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="57930-104">browserSyncSetting 枚举类型</span><span class="sxs-lookup"><span data-stu-id="57930-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="57930-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57930-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57930-107">允许 (未配置) 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。</span><span class="sxs-lookup"><span data-stu-id="57930-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="57930-108">选项可阻止跨设备同步, 但允许用户重写。</span><span class="sxs-lookup"><span data-stu-id="57930-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="57930-109">成员</span><span class="sxs-lookup"><span data-stu-id="57930-109">Members</span></span>
|<span data-ttu-id="57930-110">成员</span><span class="sxs-lookup"><span data-stu-id="57930-110">Member</span></span>|<span data-ttu-id="57930-111">值</span><span class="sxs-lookup"><span data-stu-id="57930-111">Value</span></span>|<span data-ttu-id="57930-112">说明</span><span class="sxs-lookup"><span data-stu-id="57930-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57930-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="57930-113">notConfigured</span></span>|<span data-ttu-id="57930-114">0</span><span class="sxs-lookup"><span data-stu-id="57930-114">0</span></span>|<span data-ttu-id="57930-115">默认值–允许跨设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="57930-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="57930-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="57930-116">blockedWithUserOverride</span></span>|<span data-ttu-id="57930-117">1</span><span class="sxs-lookup"><span data-stu-id="57930-117">1</span></span>|<span data-ttu-id="57930-118">阻止跨用户设备同步浏览器设置, 允许用户重写设置。</span><span class="sxs-lookup"><span data-stu-id="57930-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="57930-119">已阻止</span><span class="sxs-lookup"><span data-stu-id="57930-119">blocked</span></span>|<span data-ttu-id="57930-120">双面</span><span class="sxs-lookup"><span data-stu-id="57930-120">2</span></span>|<span data-ttu-id="57930-121">绝对阻止跨用户设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="57930-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|




