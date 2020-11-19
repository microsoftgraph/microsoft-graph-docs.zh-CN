---
title: resultantAppState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 972b708ab760d78f4fc73302cd2b8ab7e627cdb3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306602"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="dc0c2-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dc0c2-103">resultantAppState enum type</span></span>

<span data-ttu-id="dc0c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc0c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc0c2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc0c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc0c2-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dc0c2-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="dc0c2-108">成员</span><span class="sxs-lookup"><span data-stu-id="dc0c2-108">Members</span></span>
|<span data-ttu-id="dc0c2-109">成员</span><span class="sxs-lookup"><span data-stu-id="dc0c2-109">Member</span></span>|<span data-ttu-id="dc0c2-110">值</span><span class="sxs-lookup"><span data-stu-id="dc0c2-110">Value</span></span>|<span data-ttu-id="dc0c2-111">Description</span><span class="sxs-lookup"><span data-stu-id="dc0c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc0c2-112">了</span><span class="sxs-lookup"><span data-stu-id="dc0c2-112">installed</span></span>|<span data-ttu-id="dc0c2-113">1</span><span class="sxs-lookup"><span data-stu-id="dc0c2-113">1</span></span>|<span data-ttu-id="dc0c2-114">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="dc0c2-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="dc0c2-115">未能</span><span class="sxs-lookup"><span data-stu-id="dc0c2-115">failed</span></span>|<span data-ttu-id="dc0c2-116">双面</span><span class="sxs-lookup"><span data-stu-id="dc0c2-116">2</span></span>|<span data-ttu-id="dc0c2-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-117">The application failed to install.</span></span>|
|<span data-ttu-id="dc0c2-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="dc0c2-118">notInstalled</span></span>|<span data-ttu-id="dc0c2-119">第三章</span><span class="sxs-lookup"><span data-stu-id="dc0c2-119">3</span></span>|<span data-ttu-id="dc0c2-120">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-120">The application is not installed.</span></span>|
|<span data-ttu-id="dc0c2-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="dc0c2-121">uninstallFailed</span></span>|<span data-ttu-id="dc0c2-122">4 </span><span class="sxs-lookup"><span data-stu-id="dc0c2-122">4</span></span>|<span data-ttu-id="dc0c2-123">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="dc0c2-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="dc0c2-124">pendingInstall</span></span>|<span data-ttu-id="dc0c2-125">5 </span><span class="sxs-lookup"><span data-stu-id="dc0c2-125">5</span></span>|<span data-ttu-id="dc0c2-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="dc0c2-127">unknown</span><span class="sxs-lookup"><span data-stu-id="dc0c2-127">unknown</span></span>|<span data-ttu-id="dc0c2-128">99</span><span class="sxs-lookup"><span data-stu-id="dc0c2-128">99</span></span>|<span data-ttu-id="dc0c2-129">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="dc0c2-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="dc0c2-130">notApplicable</span></span>|<span data-ttu-id="dc0c2-131">-1</span><span class="sxs-lookup"><span data-stu-id="dc0c2-131">-1</span></span>|<span data-ttu-id="dc0c2-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="dc0c2-132">The application is not applicable.</span></span>|




