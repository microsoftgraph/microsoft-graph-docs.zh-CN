---
title: resultantAppState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7a364945e3b494c26873cdcc9bc4bb618e89f40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572953"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="7cda9-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7cda9-103">resultantAppState enum type</span></span>

> <span data-ttu-id="7cda9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7cda9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cda9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7cda9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cda9-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7cda9-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="7cda9-107">成员</span><span class="sxs-lookup"><span data-stu-id="7cda9-107">Members</span></span>
|<span data-ttu-id="7cda9-108">成员</span><span class="sxs-lookup"><span data-stu-id="7cda9-108">Member</span></span>|<span data-ttu-id="7cda9-109">值</span><span class="sxs-lookup"><span data-stu-id="7cda9-109">Value</span></span>|<span data-ttu-id="7cda9-110">说明</span><span class="sxs-lookup"><span data-stu-id="7cda9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cda9-111">了</span><span class="sxs-lookup"><span data-stu-id="7cda9-111">installed</span></span>|<span data-ttu-id="7cda9-112">1</span><span class="sxs-lookup"><span data-stu-id="7cda9-112">1</span></span>|<span data-ttu-id="7cda9-113">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="7cda9-113">The application is installed with no errors</span></span>|
|<span data-ttu-id="7cda9-114">未能</span><span class="sxs-lookup"><span data-stu-id="7cda9-114">failed</span></span>|<span data-ttu-id="7cda9-115">2 </span><span class="sxs-lookup"><span data-stu-id="7cda9-115">2</span></span>|<span data-ttu-id="7cda9-116">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="7cda9-116">The application failed to install.</span></span>|
|<span data-ttu-id="7cda9-117">notInstalled</span><span class="sxs-lookup"><span data-stu-id="7cda9-117">notInstalled</span></span>|<span data-ttu-id="7cda9-118">3 </span><span class="sxs-lookup"><span data-stu-id="7cda9-118">3</span></span>|<span data-ttu-id="7cda9-119">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="7cda9-119">The application is not installed.</span></span>|
|<span data-ttu-id="7cda9-120">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="7cda9-120">uninstallFailed</span></span>|<span data-ttu-id="7cda9-121">4 </span><span class="sxs-lookup"><span data-stu-id="7cda9-121">4</span></span>|<span data-ttu-id="7cda9-122">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="7cda9-122">The application failed to uninstall.</span></span>|
|<span data-ttu-id="7cda9-123">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="7cda9-123">pendingInstall</span></span>|<span data-ttu-id="7cda9-124">5 </span><span class="sxs-lookup"><span data-stu-id="7cda9-124">5</span></span>|<span data-ttu-id="7cda9-125">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="7cda9-125">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="7cda9-126">unknown</span><span class="sxs-lookup"><span data-stu-id="7cda9-126">unknown</span></span>|<span data-ttu-id="7cda9-127">99</span><span class="sxs-lookup"><span data-stu-id="7cda9-127">99</span></span>|<span data-ttu-id="7cda9-128">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="7cda9-128">The status of the application is unknown.</span></span>|
|<span data-ttu-id="7cda9-129">notApplicable</span><span class="sxs-lookup"><span data-stu-id="7cda9-129">notApplicable</span></span>|<span data-ttu-id="7cda9-130">-1</span><span class="sxs-lookup"><span data-stu-id="7cda9-130">-1</span></span>|<span data-ttu-id="7cda9-131">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="7cda9-131">The application is not applicable.</span></span>|




