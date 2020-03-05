---
title: installState 枚举类型
description: 安装状态的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e5716229ac81dc8311b2a156a774cea938a576b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489130"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="3869e-103">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3869e-103">installState enum type</span></span>

<span data-ttu-id="3869e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3869e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3869e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3869e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3869e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3869e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3869e-107">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="3869e-107">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="3869e-108">成员</span><span class="sxs-lookup"><span data-stu-id="3869e-108">Members</span></span>
|<span data-ttu-id="3869e-109">成员</span><span class="sxs-lookup"><span data-stu-id="3869e-109">Member</span></span>|<span data-ttu-id="3869e-110">值</span><span class="sxs-lookup"><span data-stu-id="3869e-110">Value</span></span>|<span data-ttu-id="3869e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3869e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3869e-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="3869e-112">notApplicable</span></span>|<span data-ttu-id="3869e-113">0</span><span class="sxs-lookup"><span data-stu-id="3869e-113">0</span></span>|<span data-ttu-id="3869e-114">不适用。</span><span class="sxs-lookup"><span data-stu-id="3869e-114">Not Applicable.</span></span>|
|<span data-ttu-id="3869e-115">了</span><span class="sxs-lookup"><span data-stu-id="3869e-115">installed</span></span>|<span data-ttu-id="3869e-116">1 </span><span class="sxs-lookup"><span data-stu-id="3869e-116">1</span></span>|<span data-ttu-id="3869e-117">了.</span><span class="sxs-lookup"><span data-stu-id="3869e-117">Installed.</span></span>|
|<span data-ttu-id="3869e-118">未能</span><span class="sxs-lookup"><span data-stu-id="3869e-118">failed</span></span>|<span data-ttu-id="3869e-119">2 </span><span class="sxs-lookup"><span data-stu-id="3869e-119">2</span></span>|<span data-ttu-id="3869e-120">未能.</span><span class="sxs-lookup"><span data-stu-id="3869e-120">Failed.</span></span>|
|<span data-ttu-id="3869e-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="3869e-121">notInstalled</span></span>|<span data-ttu-id="3869e-122">3 </span><span class="sxs-lookup"><span data-stu-id="3869e-122">3</span></span>|<span data-ttu-id="3869e-123">未安装。</span><span class="sxs-lookup"><span data-stu-id="3869e-123">Not Installed.</span></span>|
|<span data-ttu-id="3869e-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="3869e-124">uninstallFailed</span></span>|<span data-ttu-id="3869e-125">4 </span><span class="sxs-lookup"><span data-stu-id="3869e-125">4</span></span>|<span data-ttu-id="3869e-126">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="3869e-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="3869e-127">unknown</span><span class="sxs-lookup"><span data-stu-id="3869e-127">unknown</span></span>|<span data-ttu-id="3869e-128">5 </span><span class="sxs-lookup"><span data-stu-id="3869e-128">5</span></span>|<span data-ttu-id="3869e-129">陌生.</span><span class="sxs-lookup"><span data-stu-id="3869e-129">Unknown.</span></span>|



