---
title: managedAppDeviceThreatLevel 枚举类型
description: 允许应用程序兼容的 maxium 威胁级别。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 63fa79d3ce378c64a870bb40f2491402fee34e99
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781948"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="cb671-103">managedAppDeviceThreatLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cb671-103">managedAppDeviceThreatLevel enum type</span></span>

> <span data-ttu-id="cb671-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb671-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb671-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb671-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb671-106">允许应用程序兼容的 maxium 威胁级别。</span><span class="sxs-lookup"><span data-stu-id="cb671-106">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="cb671-107">成员</span><span class="sxs-lookup"><span data-stu-id="cb671-107">Members</span></span>
|<span data-ttu-id="cb671-108">成员</span><span class="sxs-lookup"><span data-stu-id="cb671-108">Member</span></span>|<span data-ttu-id="cb671-109">值</span><span class="sxs-lookup"><span data-stu-id="cb671-109">Value</span></span>|<span data-ttu-id="cb671-110">说明</span><span class="sxs-lookup"><span data-stu-id="cb671-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb671-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cb671-111">notConfigured</span></span>|<span data-ttu-id="cb671-112">0</span><span class="sxs-lookup"><span data-stu-id="cb671-112">0</span></span>|<span data-ttu-id="cb671-113">未配置值</span><span class="sxs-lookup"><span data-stu-id="cb671-113">Value not configured</span></span>|
|<span data-ttu-id="cb671-114">加密</span><span class="sxs-lookup"><span data-stu-id="cb671-114">secured</span></span>|<span data-ttu-id="cb671-115">1</span><span class="sxs-lookup"><span data-stu-id="cb671-115">1</span></span>|<span data-ttu-id="cb671-116">设备需要无威胁</span><span class="sxs-lookup"><span data-stu-id="cb671-116">Device needs to have no threat</span></span>|
|<span data-ttu-id="cb671-117">降低</span><span class="sxs-lookup"><span data-stu-id="cb671-117">low</span></span>|<span data-ttu-id="cb671-118">双面</span><span class="sxs-lookup"><span data-stu-id="cb671-118">2</span></span>|<span data-ttu-id="cb671-119">设备需要较低的威胁。</span><span class="sxs-lookup"><span data-stu-id="cb671-119">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="cb671-120">中等</span><span class="sxs-lookup"><span data-stu-id="cb671-120">medium</span></span>|<span data-ttu-id="cb671-121">第三章</span><span class="sxs-lookup"><span data-stu-id="cb671-121">3</span></span>|<span data-ttu-id="cb671-122">设备需要的威胁不超过中型威胁。</span><span class="sxs-lookup"><span data-stu-id="cb671-122">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="cb671-123">高效</span><span class="sxs-lookup"><span data-stu-id="cb671-123">high</span></span>|<span data-ttu-id="cb671-124">4 </span><span class="sxs-lookup"><span data-stu-id="cb671-124">4</span></span>|<span data-ttu-id="cb671-125">设备需要的威胁不超过高</span><span class="sxs-lookup"><span data-stu-id="cb671-125">Device needs to have not more than high threat</span></span>|



