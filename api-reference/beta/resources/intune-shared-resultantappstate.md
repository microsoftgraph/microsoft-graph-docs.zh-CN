---
title: resultantAppState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7a364945e3b494c26873cdcc9bc4bb618e89f40
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166617"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="68ee3-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="68ee3-103">resultantAppState enum type</span></span>

> <span data-ttu-id="68ee3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68ee3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68ee3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68ee3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68ee3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="68ee3-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="68ee3-107">成员</span><span class="sxs-lookup"><span data-stu-id="68ee3-107">Members</span></span>
|<span data-ttu-id="68ee3-108">成员</span><span class="sxs-lookup"><span data-stu-id="68ee3-108">Member</span></span>|<span data-ttu-id="68ee3-109">值</span><span class="sxs-lookup"><span data-stu-id="68ee3-109">Value</span></span>|<span data-ttu-id="68ee3-110">说明</span><span class="sxs-lookup"><span data-stu-id="68ee3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68ee3-111">了</span><span class="sxs-lookup"><span data-stu-id="68ee3-111">installed</span></span>|<span data-ttu-id="68ee3-112">1</span><span class="sxs-lookup"><span data-stu-id="68ee3-112">1</span></span>|<span data-ttu-id="68ee3-113">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="68ee3-113">The application is installed with no errors</span></span>|
|<span data-ttu-id="68ee3-114">failed</span><span class="sxs-lookup"><span data-stu-id="68ee3-114">failed</span></span>|<span data-ttu-id="68ee3-115">双面</span><span class="sxs-lookup"><span data-stu-id="68ee3-115">2</span></span>|<span data-ttu-id="68ee3-116">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="68ee3-116">The application failed to install.</span></span>|
|<span data-ttu-id="68ee3-117">notInstalled</span><span class="sxs-lookup"><span data-stu-id="68ee3-117">notInstalled</span></span>|<span data-ttu-id="68ee3-118">第三章</span><span class="sxs-lookup"><span data-stu-id="68ee3-118">3</span></span>|<span data-ttu-id="68ee3-119">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="68ee3-119">The application is not installed.</span></span>|
|<span data-ttu-id="68ee3-120">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="68ee3-120">uninstallFailed</span></span>|<span data-ttu-id="68ee3-121">4</span><span class="sxs-lookup"><span data-stu-id="68ee3-121">4</span></span>|<span data-ttu-id="68ee3-122">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="68ee3-122">The application failed to uninstall.</span></span>|
|<span data-ttu-id="68ee3-123">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="68ee3-123">pendingInstall</span></span>|<span data-ttu-id="68ee3-124">5</span><span class="sxs-lookup"><span data-stu-id="68ee3-124">5</span></span>|<span data-ttu-id="68ee3-125">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="68ee3-125">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="68ee3-126">unknown</span><span class="sxs-lookup"><span data-stu-id="68ee3-126">unknown</span></span>|<span data-ttu-id="68ee3-127">99</span><span class="sxs-lookup"><span data-stu-id="68ee3-127">99</span></span>|<span data-ttu-id="68ee3-128">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="68ee3-128">The status of the application is unknown.</span></span>|
|<span data-ttu-id="68ee3-129">notApplicable</span><span class="sxs-lookup"><span data-stu-id="68ee3-129">notApplicable</span></span>|<span data-ttu-id="68ee3-130">-1</span><span class="sxs-lookup"><span data-stu-id="68ee3-130">-1</span></span>|<span data-ttu-id="68ee3-131">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="68ee3-131">The application is not applicable.</span></span>|




