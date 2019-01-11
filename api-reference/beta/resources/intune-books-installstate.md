---
title: installState 枚举类型
description: 安装状态的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa281cc5f218469980a235db842e00fd8fa46647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868619"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="0d6ac-103">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0d6ac-103">installState enum type</span></span>

> <span data-ttu-id="0d6ac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d6ac-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d6ac-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d6ac-107">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="0d6ac-108">成员</span><span class="sxs-lookup"><span data-stu-id="0d6ac-108">Members</span></span>
|<span data-ttu-id="0d6ac-109">成员</span><span class="sxs-lookup"><span data-stu-id="0d6ac-109">Member</span></span>|<span data-ttu-id="0d6ac-110">值</span><span class="sxs-lookup"><span data-stu-id="0d6ac-110">Value</span></span>|<span data-ttu-id="0d6ac-111">Description</span><span class="sxs-lookup"><span data-stu-id="0d6ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d6ac-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="0d6ac-112">notApplicable</span></span>|<span data-ttu-id="0d6ac-113">0</span><span class="sxs-lookup"><span data-stu-id="0d6ac-113">0</span></span>|<span data-ttu-id="0d6ac-114">不适用。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-114">Not Applicable.</span></span>|
|<span data-ttu-id="0d6ac-115">安装</span><span class="sxs-lookup"><span data-stu-id="0d6ac-115">installed</span></span>|<span data-ttu-id="0d6ac-116">1</span><span class="sxs-lookup"><span data-stu-id="0d6ac-116">1</span></span>|<span data-ttu-id="0d6ac-117">安装。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-117">Installed.</span></span>|
|<span data-ttu-id="0d6ac-118">failed</span><span class="sxs-lookup"><span data-stu-id="0d6ac-118">failed</span></span>|<span data-ttu-id="0d6ac-119">2</span><span class="sxs-lookup"><span data-stu-id="0d6ac-119">2</span></span>|<span data-ttu-id="0d6ac-120">失败。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-120">Failed.</span></span>|
|<span data-ttu-id="0d6ac-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="0d6ac-121">notInstalled</span></span>|<span data-ttu-id="0d6ac-122">3</span><span class="sxs-lookup"><span data-stu-id="0d6ac-122">3</span></span>|<span data-ttu-id="0d6ac-123">未安装。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-123">Not Installed.</span></span>|
|<span data-ttu-id="0d6ac-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="0d6ac-124">uninstallFailed</span></span>|<span data-ttu-id="0d6ac-125">4</span><span class="sxs-lookup"><span data-stu-id="0d6ac-125">4</span></span>|<span data-ttu-id="0d6ac-126">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="0d6ac-127">unknown</span><span class="sxs-lookup"><span data-stu-id="0d6ac-127">unknown</span></span>|<span data-ttu-id="0d6ac-128">5</span><span class="sxs-lookup"><span data-stu-id="0d6ac-128">5</span></span>|<span data-ttu-id="0d6ac-129">未知。</span><span class="sxs-lookup"><span data-stu-id="0d6ac-129">Unknown.</span></span>|





