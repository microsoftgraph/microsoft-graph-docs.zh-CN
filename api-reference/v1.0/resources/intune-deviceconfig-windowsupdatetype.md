---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d7630e3cac3702380da07c2a92857d9f2786810a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027571"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="cb8ab-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cb8ab-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="cb8ab-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb8ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb8ab-105">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="cb8ab-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="cb8ab-106">成员</span><span class="sxs-lookup"><span data-stu-id="cb8ab-106">Members</span></span>
|<span data-ttu-id="cb8ab-107">成员</span><span class="sxs-lookup"><span data-stu-id="cb8ab-107">Member</span></span>|<span data-ttu-id="cb8ab-108">值</span><span class="sxs-lookup"><span data-stu-id="cb8ab-108">Value</span></span>|<span data-ttu-id="cb8ab-109">说明</span><span class="sxs-lookup"><span data-stu-id="cb8ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb8ab-110">定制</span><span class="sxs-lookup"><span data-stu-id="cb8ab-110">userDefined</span></span>|<span data-ttu-id="cb8ab-111">0</span><span class="sxs-lookup"><span data-stu-id="cb8ab-111">0</span></span>|<span data-ttu-id="cb8ab-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="cb8ab-112">Allow the user to set.</span></span>|
|<span data-ttu-id="cb8ab-113">各种</span><span class="sxs-lookup"><span data-stu-id="cb8ab-113">all</span></span>|<span data-ttu-id="cb8ab-114">1</span><span class="sxs-lookup"><span data-stu-id="cb8ab-114">1</span></span>|<span data-ttu-id="cb8ab-115">半年频道 (定向)。</span><span class="sxs-lookup"><span data-stu-id="cb8ab-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="cb8ab-116">设备从半年频道 (定向) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="cb8ab-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="cb8ab-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="cb8ab-117">businessReadyOnly</span></span>|<span data-ttu-id="cb8ab-118">双面</span><span class="sxs-lookup"><span data-stu-id="cb8ab-118">2</span></span>|<span data-ttu-id="cb8ab-119">半年频道。</span><span class="sxs-lookup"><span data-stu-id="cb8ab-119">Semi-annual Channel.</span></span> <span data-ttu-id="cb8ab-120">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="cb8ab-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="cb8ab-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="cb8ab-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="cb8ab-122">第三章</span><span class="sxs-lookup"><span data-stu-id="cb8ab-122">3</span></span>|<span data-ttu-id="cb8ab-123">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="cb8ab-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="cb8ab-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="cb8ab-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="cb8ab-125">4</span><span class="sxs-lookup"><span data-stu-id="cb8ab-125">4</span></span>|<span data-ttu-id="cb8ab-126">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="cb8ab-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="cb8ab-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="cb8ab-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="cb8ab-128">5</span><span class="sxs-lookup"><span data-stu-id="cb8ab-128">5</span></span>|<span data-ttu-id="cb8ab-129">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="cb8ab-129">Release Windows Insider build</span></span>|



