---
title: resultantAppState 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3412e630fe9bbf154207a79fe805569c04dbd628
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523567"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="a3e95-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3e95-103">resultantAppState enum type</span></span>

<span data-ttu-id="a3e95-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a3e95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3e95-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3e95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3e95-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3e95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e95-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a3e95-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="a3e95-108">成员</span><span class="sxs-lookup"><span data-stu-id="a3e95-108">Members</span></span>
|<span data-ttu-id="a3e95-109">成员</span><span class="sxs-lookup"><span data-stu-id="a3e95-109">Member</span></span>|<span data-ttu-id="a3e95-110">值</span><span class="sxs-lookup"><span data-stu-id="a3e95-110">Value</span></span>|<span data-ttu-id="a3e95-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3e95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e95-112">了</span><span class="sxs-lookup"><span data-stu-id="a3e95-112">installed</span></span>|<span data-ttu-id="a3e95-113">1 </span><span class="sxs-lookup"><span data-stu-id="a3e95-113">1</span></span>|<span data-ttu-id="a3e95-114">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="a3e95-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="a3e95-115">未能</span><span class="sxs-lookup"><span data-stu-id="a3e95-115">failed</span></span>|<span data-ttu-id="a3e95-116">2 </span><span class="sxs-lookup"><span data-stu-id="a3e95-116">2</span></span>|<span data-ttu-id="a3e95-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="a3e95-117">The application failed to install.</span></span>|
|<span data-ttu-id="a3e95-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="a3e95-118">notInstalled</span></span>|<span data-ttu-id="a3e95-119">3 </span><span class="sxs-lookup"><span data-stu-id="a3e95-119">3</span></span>|<span data-ttu-id="a3e95-120">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="a3e95-120">The application is not installed.</span></span>|
|<span data-ttu-id="a3e95-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="a3e95-121">uninstallFailed</span></span>|<span data-ttu-id="a3e95-122">4 </span><span class="sxs-lookup"><span data-stu-id="a3e95-122">4</span></span>|<span data-ttu-id="a3e95-123">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="a3e95-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="a3e95-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="a3e95-124">pendingInstall</span></span>|<span data-ttu-id="a3e95-125">5 </span><span class="sxs-lookup"><span data-stu-id="a3e95-125">5</span></span>|<span data-ttu-id="a3e95-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="a3e95-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="a3e95-127">unknown</span><span class="sxs-lookup"><span data-stu-id="a3e95-127">unknown</span></span>|<span data-ttu-id="a3e95-128">99</span><span class="sxs-lookup"><span data-stu-id="a3e95-128">99</span></span>|<span data-ttu-id="a3e95-129">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="a3e95-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="a3e95-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="a3e95-130">notApplicable</span></span>|<span data-ttu-id="a3e95-131">-1</span><span class="sxs-lookup"><span data-stu-id="a3e95-131">-1</span></span>|<span data-ttu-id="a3e95-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="a3e95-132">The application is not applicable.</span></span>|



