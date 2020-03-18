---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 402feb76fbb95664f5b4fe8190dfb71504db0abf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791875"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="de5ca-103">edgeKioskModeRestrictionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="de5ca-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="de5ca-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de5ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de5ca-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de5ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de5ca-106">根据展台模式指定 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="de5ca-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="de5ca-107">成员</span><span class="sxs-lookup"><span data-stu-id="de5ca-107">Members</span></span>
|<span data-ttu-id="de5ca-108">成员</span><span class="sxs-lookup"><span data-stu-id="de5ca-108">Member</span></span>|<span data-ttu-id="de5ca-109">值</span><span class="sxs-lookup"><span data-stu-id="de5ca-109">Value</span></span>|<span data-ttu-id="de5ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="de5ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de5ca-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="de5ca-111">notConfigured</span></span>|<span data-ttu-id="de5ca-112">0</span><span class="sxs-lookup"><span data-stu-id="de5ca-112">0</span></span>|<span data-ttu-id="de5ca-113">未配置（无限制）。</span><span class="sxs-lookup"><span data-stu-id="de5ca-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="de5ca-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="de5ca-114">digitalSignage</span></span>|<span data-ttu-id="de5ca-115">1</span><span class="sxs-lookup"><span data-stu-id="de5ca-115">1</span></span>|<span data-ttu-id="de5ca-116">单应用模式中的交互/数字告示。</span><span class="sxs-lookup"><span data-stu-id="de5ca-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="de5ca-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="de5ca-117">normalMode</span></span>|<span data-ttu-id="de5ca-118">双面</span><span class="sxs-lookup"><span data-stu-id="de5ca-118">2</span></span>|<span data-ttu-id="de5ca-119">正常模式（Microsoft Edge 的完整版本）。</span><span class="sxs-lookup"><span data-stu-id="de5ca-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="de5ca-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="de5ca-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="de5ca-121">第三章</span><span class="sxs-lookup"><span data-stu-id="de5ca-121">3</span></span>|<span data-ttu-id="de5ca-122">单应用模式中的公共浏览。</span><span class="sxs-lookup"><span data-stu-id="de5ca-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="de5ca-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="de5ca-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="de5ca-124">4 </span><span class="sxs-lookup"><span data-stu-id="de5ca-124">4</span></span>|<span data-ttu-id="de5ca-125">多应用模式中的公共浏览（inPrivate）。</span><span class="sxs-lookup"><span data-stu-id="de5ca-125">Public browsing (inPrivate) in multi-app mode.</span></span>|



