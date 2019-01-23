---
title: browserSyncSetting 枚举类型
description: Allow(Not Configured) 或 prevent(Block) Microsoft 边缘浏览器设置同步。 选项可以防止同步跨设备，但允许用户替代。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431320"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="f6f7c-104">browserSyncSetting 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f6f7c-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="f6f7c-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6f7c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6f7c-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f7c-108">Allow(Not Configured) 或 prevent(Block) Microsoft 边缘浏览器设置同步。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="f6f7c-109">选项可以防止同步跨设备，但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="f6f7c-110">成员</span><span class="sxs-lookup"><span data-stu-id="f6f7c-110">Members</span></span>
|<span data-ttu-id="f6f7c-111">成员</span><span class="sxs-lookup"><span data-stu-id="f6f7c-111">Member</span></span>|<span data-ttu-id="f6f7c-112">值</span><span class="sxs-lookup"><span data-stu-id="f6f7c-112">Value</span></span>|<span data-ttu-id="f6f7c-113">说明</span><span class="sxs-lookup"><span data-stu-id="f6f7c-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6f7c-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f6f7c-114">notConfigured</span></span>|<span data-ttu-id="f6f7c-115">0</span><span class="sxs-lookup"><span data-stu-id="f6f7c-115">0</span></span>|<span data-ttu-id="f6f7c-116">默认值 – 允许跨设备同步的浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="f6f7c-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="f6f7c-117">blockedWithUserOverride</span></span>|<span data-ttu-id="f6f7c-118">1</span><span class="sxs-lookup"><span data-stu-id="f6f7c-118">1</span></span>|<span data-ttu-id="f6f7c-119">防止跨用户设备同步的浏览器设置时，允许用户替代的设置。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="f6f7c-120">已阻止</span><span class="sxs-lookup"><span data-stu-id="f6f7c-120">blocked</span></span>|<span data-ttu-id="f6f7c-121">2</span><span class="sxs-lookup"><span data-stu-id="f6f7c-121">2</span></span>|<span data-ttu-id="f6f7c-122">绝对防止跨用户设备同步的浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="f6f7c-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




