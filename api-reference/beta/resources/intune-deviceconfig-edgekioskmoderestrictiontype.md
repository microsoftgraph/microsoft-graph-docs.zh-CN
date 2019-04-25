---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74b03555456c058411c9a50c7392f29fe60d3aed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524510"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="a7045-103">edgeKioskModeRestrictionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a7045-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="a7045-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7045-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7045-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7045-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7045-106">根据展台模式指定 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="a7045-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="a7045-107">成员</span><span class="sxs-lookup"><span data-stu-id="a7045-107">Members</span></span>
|<span data-ttu-id="a7045-108">成员</span><span class="sxs-lookup"><span data-stu-id="a7045-108">Member</span></span>|<span data-ttu-id="a7045-109">值</span><span class="sxs-lookup"><span data-stu-id="a7045-109">Value</span></span>|<span data-ttu-id="a7045-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7045-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7045-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a7045-111">notConfigured</span></span>|<span data-ttu-id="a7045-112">0</span><span class="sxs-lookup"><span data-stu-id="a7045-112">0</span></span>|<span data-ttu-id="a7045-113">未配置 (无限制)。</span><span class="sxs-lookup"><span data-stu-id="a7045-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="a7045-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="a7045-114">digitalSignage</span></span>|<span data-ttu-id="a7045-115">1</span><span class="sxs-lookup"><span data-stu-id="a7045-115">1</span></span>|<span data-ttu-id="a7045-116">单应用模式中的交互/数字告示。</span><span class="sxs-lookup"><span data-stu-id="a7045-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="a7045-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="a7045-117">normalMode</span></span>|<span data-ttu-id="a7045-118">2 </span><span class="sxs-lookup"><span data-stu-id="a7045-118">2</span></span>|<span data-ttu-id="a7045-119">正常模式 (Microsoft Edge 的完整版本)。</span><span class="sxs-lookup"><span data-stu-id="a7045-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="a7045-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="a7045-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="a7045-121">3 </span><span class="sxs-lookup"><span data-stu-id="a7045-121">3</span></span>|<span data-ttu-id="a7045-122">单应用模式中的公共浏览。</span><span class="sxs-lookup"><span data-stu-id="a7045-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="a7045-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="a7045-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="a7045-124">4 </span><span class="sxs-lookup"><span data-stu-id="a7045-124">4</span></span>|<span data-ttu-id="a7045-125">多应用模式中的公共浏览 (inPrivate)。</span><span class="sxs-lookup"><span data-stu-id="a7045-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





