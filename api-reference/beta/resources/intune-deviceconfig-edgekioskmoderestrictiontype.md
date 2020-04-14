---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1dfd86f9bd3a35e82f5210294c9b0648a4bab228
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386266"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="afa27-103">edgeKioskModeRestrictionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="afa27-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="afa27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afa27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afa27-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="afa27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afa27-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afa27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afa27-107">根据展台模式指定 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="afa27-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="afa27-108">成员</span><span class="sxs-lookup"><span data-stu-id="afa27-108">Members</span></span>
|<span data-ttu-id="afa27-109">成员</span><span class="sxs-lookup"><span data-stu-id="afa27-109">Member</span></span>|<span data-ttu-id="afa27-110">值</span><span class="sxs-lookup"><span data-stu-id="afa27-110">Value</span></span>|<span data-ttu-id="afa27-111">说明</span><span class="sxs-lookup"><span data-stu-id="afa27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afa27-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="afa27-112">notConfigured</span></span>|<span data-ttu-id="afa27-113">0</span><span class="sxs-lookup"><span data-stu-id="afa27-113">0</span></span>|<span data-ttu-id="afa27-114">未配置（无限制）。</span><span class="sxs-lookup"><span data-stu-id="afa27-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="afa27-115">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="afa27-115">digitalSignage</span></span>|<span data-ttu-id="afa27-116">1</span><span class="sxs-lookup"><span data-stu-id="afa27-116">1</span></span>|<span data-ttu-id="afa27-117">单应用模式中的交互/数字告示。</span><span class="sxs-lookup"><span data-stu-id="afa27-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="afa27-118">normalMode</span><span class="sxs-lookup"><span data-stu-id="afa27-118">normalMode</span></span>|<span data-ttu-id="afa27-119">双面</span><span class="sxs-lookup"><span data-stu-id="afa27-119">2</span></span>|<span data-ttu-id="afa27-120">正常模式（Microsoft Edge 的完整版本）。</span><span class="sxs-lookup"><span data-stu-id="afa27-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="afa27-121">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="afa27-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="afa27-122">第三章</span><span class="sxs-lookup"><span data-stu-id="afa27-122">3</span></span>|<span data-ttu-id="afa27-123">单应用模式中的公共浏览。</span><span class="sxs-lookup"><span data-stu-id="afa27-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="afa27-124">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="afa27-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="afa27-125">4 </span><span class="sxs-lookup"><span data-stu-id="afa27-125">4</span></span>|<span data-ttu-id="afa27-126">多应用模式中的公共浏览（inPrivate）。</span><span class="sxs-lookup"><span data-stu-id="afa27-126">Public browsing (inPrivate) in multi-app mode.</span></span>|



