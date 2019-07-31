---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbd3d13ad39b6acda5fd67d69c8cb2de2f2e7c55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001465"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="3f31c-103">edgeKioskModeRestrictionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3f31c-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="3f31c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f31c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f31c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f31c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f31c-106">根据展台模式指定 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="3f31c-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="3f31c-107">成员</span><span class="sxs-lookup"><span data-stu-id="3f31c-107">Members</span></span>
|<span data-ttu-id="3f31c-108">成员</span><span class="sxs-lookup"><span data-stu-id="3f31c-108">Member</span></span>|<span data-ttu-id="3f31c-109">值</span><span class="sxs-lookup"><span data-stu-id="3f31c-109">Value</span></span>|<span data-ttu-id="3f31c-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f31c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f31c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3f31c-111">notConfigured</span></span>|<span data-ttu-id="3f31c-112">0</span><span class="sxs-lookup"><span data-stu-id="3f31c-112">0</span></span>|<span data-ttu-id="3f31c-113">未配置 (无限制)。</span><span class="sxs-lookup"><span data-stu-id="3f31c-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="3f31c-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="3f31c-114">digitalSignage</span></span>|<span data-ttu-id="3f31c-115">1</span><span class="sxs-lookup"><span data-stu-id="3f31c-115">1</span></span>|<span data-ttu-id="3f31c-116">单应用模式中的交互/数字告示。</span><span class="sxs-lookup"><span data-stu-id="3f31c-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="3f31c-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="3f31c-117">normalMode</span></span>|<span data-ttu-id="3f31c-118">双面</span><span class="sxs-lookup"><span data-stu-id="3f31c-118">2</span></span>|<span data-ttu-id="3f31c-119">正常模式 (Microsoft Edge 的完整版本)。</span><span class="sxs-lookup"><span data-stu-id="3f31c-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="3f31c-120">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="3f31c-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="3f31c-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3f31c-121">3</span></span>|<span data-ttu-id="3f31c-122">单应用模式中的公共浏览。</span><span class="sxs-lookup"><span data-stu-id="3f31c-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="3f31c-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="3f31c-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="3f31c-124">4</span><span class="sxs-lookup"><span data-stu-id="3f31c-124">4</span></span>|<span data-ttu-id="3f31c-125">多应用模式中的公共浏览 (inPrivate)。</span><span class="sxs-lookup"><span data-stu-id="3f31c-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





