---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98508a288ef46f8112ac5d796b8ddef64c5940e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058198"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="f65e4-103">edgeKioskModeRestrictionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f65e4-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="f65e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f65e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f65e4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f65e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f65e4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f65e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f65e4-107">根据展台模式指定 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="f65e4-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="f65e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="f65e4-108">Members</span></span>
|<span data-ttu-id="f65e4-109">成员</span><span class="sxs-lookup"><span data-stu-id="f65e4-109">Member</span></span>|<span data-ttu-id="f65e4-110">值</span><span class="sxs-lookup"><span data-stu-id="f65e4-110">Value</span></span>|<span data-ttu-id="f65e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="f65e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f65e4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f65e4-112">notConfigured</span></span>|<span data-ttu-id="f65e4-113">0</span><span class="sxs-lookup"><span data-stu-id="f65e4-113">0</span></span>|<span data-ttu-id="f65e4-114">未 (不受限制的) 配置。</span><span class="sxs-lookup"><span data-stu-id="f65e4-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="f65e4-115">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="f65e4-115">digitalSignage</span></span>|<span data-ttu-id="f65e4-116">1 </span><span class="sxs-lookup"><span data-stu-id="f65e4-116">1</span></span>|<span data-ttu-id="f65e4-117">单应用模式中的交互/数字告示。</span><span class="sxs-lookup"><span data-stu-id="f65e4-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="f65e4-118">normalMode</span><span class="sxs-lookup"><span data-stu-id="f65e4-118">normalMode</span></span>|<span data-ttu-id="f65e4-119">2 </span><span class="sxs-lookup"><span data-stu-id="f65e4-119">2</span></span>|<span data-ttu-id="f65e4-120">正常模式 (Microsoft Edge) 的完整版本。</span><span class="sxs-lookup"><span data-stu-id="f65e4-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="f65e4-121">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="f65e4-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="f65e4-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f65e4-122">3</span></span>|<span data-ttu-id="f65e4-123">单应用模式中的公共浏览。</span><span class="sxs-lookup"><span data-stu-id="f65e4-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="f65e4-124">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="f65e4-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="f65e4-125">4 </span><span class="sxs-lookup"><span data-stu-id="f65e4-125">4</span></span>|<span data-ttu-id="f65e4-126">在多应用模式下，公共浏览 (inPrivate) 。</span><span class="sxs-lookup"><span data-stu-id="f65e4-126">Public browsing (inPrivate) in multi-app mode.</span></span>|






