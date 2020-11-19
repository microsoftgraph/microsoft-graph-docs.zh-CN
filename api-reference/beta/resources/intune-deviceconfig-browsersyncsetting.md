---
title: browserSyncSetting 枚举类型
description: 允许未配置 () 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。 选项可阻止跨设备同步，但允许用户重写。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 74803f708fdf9f66c7b903c22cecf23cb06ae8dc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260500"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="ac7c4-104">browserSyncSetting 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ac7c4-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="ac7c4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac7c4-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac7c4-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac7c4-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac7c4-108">允许未配置 () 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="ac7c4-109">选项可阻止跨设备同步，但允许用户重写。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="ac7c4-110">成员</span><span class="sxs-lookup"><span data-stu-id="ac7c4-110">Members</span></span>
|<span data-ttu-id="ac7c4-111">成员</span><span class="sxs-lookup"><span data-stu-id="ac7c4-111">Member</span></span>|<span data-ttu-id="ac7c4-112">值</span><span class="sxs-lookup"><span data-stu-id="ac7c4-112">Value</span></span>|<span data-ttu-id="ac7c4-113">说明</span><span class="sxs-lookup"><span data-stu-id="ac7c4-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac7c4-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ac7c4-114">notConfigured</span></span>|<span data-ttu-id="ac7c4-115">0</span><span class="sxs-lookup"><span data-stu-id="ac7c4-115">0</span></span>|<span data-ttu-id="ac7c4-116">默认值–允许跨设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="ac7c4-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="ac7c4-117">blockedWithUserOverride</span></span>|<span data-ttu-id="ac7c4-118">1</span><span class="sxs-lookup"><span data-stu-id="ac7c4-118">1</span></span>|<span data-ttu-id="ac7c4-119">阻止跨用户设备同步浏览器设置，允许用户重写设置。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="ac7c4-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="ac7c4-120">blocked</span></span>|<span data-ttu-id="ac7c4-121">双面</span><span class="sxs-lookup"><span data-stu-id="ac7c4-121">2</span></span>|<span data-ttu-id="ac7c4-122">绝对阻止跨用户设备同步浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="ac7c4-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




