---
title: macOSSoftwareUpdateDelayPolicy 枚举类型
description: 标记 enum 以确定是否延迟 macOS 的软件更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2f9d9100fc7bad05a6fd8d48a90a07cd268d0977
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731090"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a><span data-ttu-id="503ab-103">macOSSoftwareUpdateDelayPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="503ab-103">macOSSoftwareUpdateDelayPolicy enum type</span></span>

<span data-ttu-id="503ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="503ab-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="503ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="503ab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="503ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="503ab-107">标记 enum 以确定是否延迟 macOS 的软件更新。</span><span class="sxs-lookup"><span data-stu-id="503ab-107">Flag enum to determine whether to delay software updates for macOS.</span></span>

## <a name="members"></a><span data-ttu-id="503ab-108">成员</span><span class="sxs-lookup"><span data-stu-id="503ab-108">Members</span></span>
|<span data-ttu-id="503ab-109">成员</span><span class="sxs-lookup"><span data-stu-id="503ab-109">Member</span></span>|<span data-ttu-id="503ab-110">值</span><span class="sxs-lookup"><span data-stu-id="503ab-110">Value</span></span>|<span data-ttu-id="503ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="503ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503ab-112">无</span><span class="sxs-lookup"><span data-stu-id="503ab-112">none</span></span>|<span data-ttu-id="503ab-113">0</span><span class="sxs-lookup"><span data-stu-id="503ab-113">0</span></span>|<span data-ttu-id="503ab-114">将不会强制执行软件更新延迟。</span><span class="sxs-lookup"><span data-stu-id="503ab-114">Software update delays will not be enforced.</span></span>|
|<span data-ttu-id="503ab-115">delayOSUpdateVisibility</span><span class="sxs-lookup"><span data-stu-id="503ab-115">delayOSUpdateVisibility</span></span>|<span data-ttu-id="503ab-116">1</span><span class="sxs-lookup"><span data-stu-id="503ab-116">1</span></span>|<span data-ttu-id="503ab-117">对 OS 软件更新强制延迟。</span><span class="sxs-lookup"><span data-stu-id="503ab-117">Force delays for OS software updates.</span></span>|
|<span data-ttu-id="503ab-118">delayAppUpdateVisibility</span><span class="sxs-lookup"><span data-stu-id="503ab-118">delayAppUpdateVisibility</span></span>|<span data-ttu-id="503ab-119">双面</span><span class="sxs-lookup"><span data-stu-id="503ab-119">2</span></span>|<span data-ttu-id="503ab-120">对应用软件更新强制延迟。</span><span class="sxs-lookup"><span data-stu-id="503ab-120">Force delays for app software updates.</span></span>|





