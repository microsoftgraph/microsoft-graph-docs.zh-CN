---
title: resultantAppState 枚举类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 99aece736483466a488fd3a301381ba0f26c64a5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767923"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="e539e-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e539e-103">resultantAppState enum type</span></span>

> <span data-ttu-id="e539e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e539e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e539e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e539e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e539e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e539e-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e539e-107">成员</span><span class="sxs-lookup"><span data-stu-id="e539e-107">Members</span></span>
|<span data-ttu-id="e539e-108">成员</span><span class="sxs-lookup"><span data-stu-id="e539e-108">Member</span></span>|<span data-ttu-id="e539e-109">值</span><span class="sxs-lookup"><span data-stu-id="e539e-109">Value</span></span>|<span data-ttu-id="e539e-110">说明</span><span class="sxs-lookup"><span data-stu-id="e539e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e539e-111">了</span><span class="sxs-lookup"><span data-stu-id="e539e-111">installed</span></span>|<span data-ttu-id="e539e-112">1</span><span class="sxs-lookup"><span data-stu-id="e539e-112">1</span></span>|<span data-ttu-id="e539e-113">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="e539e-113">The application is installed with no errors</span></span>|
|<span data-ttu-id="e539e-114">未能</span><span class="sxs-lookup"><span data-stu-id="e539e-114">failed</span></span>|<span data-ttu-id="e539e-115">双面</span><span class="sxs-lookup"><span data-stu-id="e539e-115">2</span></span>|<span data-ttu-id="e539e-116">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="e539e-116">The application failed to install.</span></span>|
|<span data-ttu-id="e539e-117">notInstalled</span><span class="sxs-lookup"><span data-stu-id="e539e-117">notInstalled</span></span>|<span data-ttu-id="e539e-118">第三章</span><span class="sxs-lookup"><span data-stu-id="e539e-118">3</span></span>|<span data-ttu-id="e539e-119">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="e539e-119">The application is not installed.</span></span>|
|<span data-ttu-id="e539e-120">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="e539e-120">uninstallFailed</span></span>|<span data-ttu-id="e539e-121">4 </span><span class="sxs-lookup"><span data-stu-id="e539e-121">4</span></span>|<span data-ttu-id="e539e-122">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="e539e-122">The application failed to uninstall.</span></span>|
|<span data-ttu-id="e539e-123">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="e539e-123">pendingInstall</span></span>|<span data-ttu-id="e539e-124">5 </span><span class="sxs-lookup"><span data-stu-id="e539e-124">5</span></span>|<span data-ttu-id="e539e-125">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="e539e-125">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="e539e-126">unknown</span><span class="sxs-lookup"><span data-stu-id="e539e-126">unknown</span></span>|<span data-ttu-id="e539e-127">99</span><span class="sxs-lookup"><span data-stu-id="e539e-127">99</span></span>|<span data-ttu-id="e539e-128">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="e539e-128">The status of the application is unknown.</span></span>|
|<span data-ttu-id="e539e-129">notApplicable</span><span class="sxs-lookup"><span data-stu-id="e539e-129">notApplicable</span></span>|<span data-ttu-id="e539e-130">-1</span><span class="sxs-lookup"><span data-stu-id="e539e-130">-1</span></span>|<span data-ttu-id="e539e-131">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="e539e-131">The application is not applicable.</span></span>|



