---
title: resultantAppState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a4b50a903dc60e9f6d152c0b11f55811f85c446
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473527"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="557ad-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="557ad-103">resultantAppState enum type</span></span>

<span data-ttu-id="557ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="557ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="557ad-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="557ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="557ad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="557ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="557ad-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="557ad-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="557ad-108">成员</span><span class="sxs-lookup"><span data-stu-id="557ad-108">Members</span></span>
|<span data-ttu-id="557ad-109">成员</span><span class="sxs-lookup"><span data-stu-id="557ad-109">Member</span></span>|<span data-ttu-id="557ad-110">值</span><span class="sxs-lookup"><span data-stu-id="557ad-110">Value</span></span>|<span data-ttu-id="557ad-111">说明</span><span class="sxs-lookup"><span data-stu-id="557ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="557ad-112">了</span><span class="sxs-lookup"><span data-stu-id="557ad-112">installed</span></span>|<span data-ttu-id="557ad-113">1</span><span class="sxs-lookup"><span data-stu-id="557ad-113">1</span></span>|<span data-ttu-id="557ad-114">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="557ad-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="557ad-115">未能</span><span class="sxs-lookup"><span data-stu-id="557ad-115">failed</span></span>|<span data-ttu-id="557ad-116">双面</span><span class="sxs-lookup"><span data-stu-id="557ad-116">2</span></span>|<span data-ttu-id="557ad-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="557ad-117">The application failed to install.</span></span>|
|<span data-ttu-id="557ad-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="557ad-118">notInstalled</span></span>|<span data-ttu-id="557ad-119">第三章</span><span class="sxs-lookup"><span data-stu-id="557ad-119">3</span></span>|<span data-ttu-id="557ad-120">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="557ad-120">The application is not installed.</span></span>|
|<span data-ttu-id="557ad-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="557ad-121">uninstallFailed</span></span>|<span data-ttu-id="557ad-122">4 </span><span class="sxs-lookup"><span data-stu-id="557ad-122">4</span></span>|<span data-ttu-id="557ad-123">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="557ad-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="557ad-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="557ad-124">pendingInstall</span></span>|<span data-ttu-id="557ad-125">5 </span><span class="sxs-lookup"><span data-stu-id="557ad-125">5</span></span>|<span data-ttu-id="557ad-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="557ad-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="557ad-127">unknown</span><span class="sxs-lookup"><span data-stu-id="557ad-127">unknown</span></span>|<span data-ttu-id="557ad-128">99</span><span class="sxs-lookup"><span data-stu-id="557ad-128">99</span></span>|<span data-ttu-id="557ad-129">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="557ad-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="557ad-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="557ad-130">notApplicable</span></span>|<span data-ttu-id="557ad-131">-1</span><span class="sxs-lookup"><span data-stu-id="557ad-131">-1</span></span>|<span data-ttu-id="557ad-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="557ad-132">The application is not applicable.</span></span>|



