---
title: installState 枚举类型
description: 安装状态的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dbe7ce024e1ddae723254c4efd2b7214a0e8990e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797386"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="940fc-103">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="940fc-103">installState enum type</span></span>

> <span data-ttu-id="940fc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="940fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="940fc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="940fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="940fc-106">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="940fc-106">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="940fc-107">成员</span><span class="sxs-lookup"><span data-stu-id="940fc-107">Members</span></span>
|<span data-ttu-id="940fc-108">成员</span><span class="sxs-lookup"><span data-stu-id="940fc-108">Member</span></span>|<span data-ttu-id="940fc-109">值</span><span class="sxs-lookup"><span data-stu-id="940fc-109">Value</span></span>|<span data-ttu-id="940fc-110">说明</span><span class="sxs-lookup"><span data-stu-id="940fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940fc-111">notApplicable</span><span class="sxs-lookup"><span data-stu-id="940fc-111">notApplicable</span></span>|<span data-ttu-id="940fc-112">0</span><span class="sxs-lookup"><span data-stu-id="940fc-112">0</span></span>|<span data-ttu-id="940fc-113">不适用。</span><span class="sxs-lookup"><span data-stu-id="940fc-113">Not Applicable.</span></span>|
|<span data-ttu-id="940fc-114">了</span><span class="sxs-lookup"><span data-stu-id="940fc-114">installed</span></span>|<span data-ttu-id="940fc-115">1</span><span class="sxs-lookup"><span data-stu-id="940fc-115">1</span></span>|<span data-ttu-id="940fc-116">了.</span><span class="sxs-lookup"><span data-stu-id="940fc-116">Installed.</span></span>|
|<span data-ttu-id="940fc-117">未能</span><span class="sxs-lookup"><span data-stu-id="940fc-117">failed</span></span>|<span data-ttu-id="940fc-118">双面</span><span class="sxs-lookup"><span data-stu-id="940fc-118">2</span></span>|<span data-ttu-id="940fc-119">未能.</span><span class="sxs-lookup"><span data-stu-id="940fc-119">Failed.</span></span>|
|<span data-ttu-id="940fc-120">notInstalled</span><span class="sxs-lookup"><span data-stu-id="940fc-120">notInstalled</span></span>|<span data-ttu-id="940fc-121">第三章</span><span class="sxs-lookup"><span data-stu-id="940fc-121">3</span></span>|<span data-ttu-id="940fc-122">未安装。</span><span class="sxs-lookup"><span data-stu-id="940fc-122">Not Installed.</span></span>|
|<span data-ttu-id="940fc-123">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="940fc-123">uninstallFailed</span></span>|<span data-ttu-id="940fc-124">4 </span><span class="sxs-lookup"><span data-stu-id="940fc-124">4</span></span>|<span data-ttu-id="940fc-125">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="940fc-125">Uninstall Failed.</span></span>|
|<span data-ttu-id="940fc-126">unknown</span><span class="sxs-lookup"><span data-stu-id="940fc-126">unknown</span></span>|<span data-ttu-id="940fc-127">5 </span><span class="sxs-lookup"><span data-stu-id="940fc-127">5</span></span>|<span data-ttu-id="940fc-128">陌生.</span><span class="sxs-lookup"><span data-stu-id="940fc-128">Unknown.</span></span>|



