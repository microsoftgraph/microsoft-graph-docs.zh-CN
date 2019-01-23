---
title: installState 枚举类型
description: 安装状态的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c3a1d86257611cb00d8ee2c4ee0b8173b03f197
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425874"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="2a1d9-103">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2a1d9-103">installState enum type</span></span>

> <span data-ttu-id="2a1d9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2a1d9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a1d9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a1d9-107">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-107">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="2a1d9-108">成员</span><span class="sxs-lookup"><span data-stu-id="2a1d9-108">Members</span></span>
|<span data-ttu-id="2a1d9-109">成员</span><span class="sxs-lookup"><span data-stu-id="2a1d9-109">Member</span></span>|<span data-ttu-id="2a1d9-110">值</span><span class="sxs-lookup"><span data-stu-id="2a1d9-110">Value</span></span>|<span data-ttu-id="2a1d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="2a1d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a1d9-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="2a1d9-112">notApplicable</span></span>|<span data-ttu-id="2a1d9-113">0</span><span class="sxs-lookup"><span data-stu-id="2a1d9-113">0</span></span>|<span data-ttu-id="2a1d9-114">不适用。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-114">Not Applicable.</span></span>|
|<span data-ttu-id="2a1d9-115">安装</span><span class="sxs-lookup"><span data-stu-id="2a1d9-115">installed</span></span>|<span data-ttu-id="2a1d9-116">1</span><span class="sxs-lookup"><span data-stu-id="2a1d9-116">1</span></span>|<span data-ttu-id="2a1d9-117">安装。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-117">Installed.</span></span>|
|<span data-ttu-id="2a1d9-118">failed</span><span class="sxs-lookup"><span data-stu-id="2a1d9-118">failed</span></span>|<span data-ttu-id="2a1d9-119">2</span><span class="sxs-lookup"><span data-stu-id="2a1d9-119">2</span></span>|<span data-ttu-id="2a1d9-120">失败。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-120">Failed.</span></span>|
|<span data-ttu-id="2a1d9-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="2a1d9-121">notInstalled</span></span>|<span data-ttu-id="2a1d9-122">3</span><span class="sxs-lookup"><span data-stu-id="2a1d9-122">3</span></span>|<span data-ttu-id="2a1d9-123">未安装。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-123">Not Installed.</span></span>|
|<span data-ttu-id="2a1d9-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="2a1d9-124">uninstallFailed</span></span>|<span data-ttu-id="2a1d9-125">4</span><span class="sxs-lookup"><span data-stu-id="2a1d9-125">4</span></span>|<span data-ttu-id="2a1d9-126">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="2a1d9-127">unknown</span><span class="sxs-lookup"><span data-stu-id="2a1d9-127">unknown</span></span>|<span data-ttu-id="2a1d9-128">5</span><span class="sxs-lookup"><span data-stu-id="2a1d9-128">5</span></span>|<span data-ttu-id="2a1d9-129">未知。</span><span class="sxs-lookup"><span data-stu-id="2a1d9-129">Unknown.</span></span>|




