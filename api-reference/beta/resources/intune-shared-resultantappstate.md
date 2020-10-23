---
title: resultantAppState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b431a4ca3b44afc54547e3dc7e02e1886c95618a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730337"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="86da0-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="86da0-103">resultantAppState enum type</span></span>

<span data-ttu-id="86da0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86da0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86da0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86da0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86da0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86da0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86da0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="86da0-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="86da0-108">成员</span><span class="sxs-lookup"><span data-stu-id="86da0-108">Members</span></span>
|<span data-ttu-id="86da0-109">成员</span><span class="sxs-lookup"><span data-stu-id="86da0-109">Member</span></span>|<span data-ttu-id="86da0-110">值</span><span class="sxs-lookup"><span data-stu-id="86da0-110">Value</span></span>|<span data-ttu-id="86da0-111">说明</span><span class="sxs-lookup"><span data-stu-id="86da0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86da0-112">了</span><span class="sxs-lookup"><span data-stu-id="86da0-112">installed</span></span>|<span data-ttu-id="86da0-113">1</span><span class="sxs-lookup"><span data-stu-id="86da0-113">1</span></span>|<span data-ttu-id="86da0-114">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="86da0-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="86da0-115">未能</span><span class="sxs-lookup"><span data-stu-id="86da0-115">failed</span></span>|<span data-ttu-id="86da0-116">双面</span><span class="sxs-lookup"><span data-stu-id="86da0-116">2</span></span>|<span data-ttu-id="86da0-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="86da0-117">The application failed to install.</span></span>|
|<span data-ttu-id="86da0-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="86da0-118">notInstalled</span></span>|<span data-ttu-id="86da0-119">第三章</span><span class="sxs-lookup"><span data-stu-id="86da0-119">3</span></span>|<span data-ttu-id="86da0-120">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="86da0-120">The application is not installed.</span></span>|
|<span data-ttu-id="86da0-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="86da0-121">uninstallFailed</span></span>|<span data-ttu-id="86da0-122">4 </span><span class="sxs-lookup"><span data-stu-id="86da0-122">4</span></span>|<span data-ttu-id="86da0-123">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="86da0-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="86da0-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="86da0-124">pendingInstall</span></span>|<span data-ttu-id="86da0-125">5 </span><span class="sxs-lookup"><span data-stu-id="86da0-125">5</span></span>|<span data-ttu-id="86da0-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="86da0-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="86da0-127">unknown</span><span class="sxs-lookup"><span data-stu-id="86da0-127">unknown</span></span>|<span data-ttu-id="86da0-128">99</span><span class="sxs-lookup"><span data-stu-id="86da0-128">99</span></span>|<span data-ttu-id="86da0-129">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="86da0-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="86da0-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="86da0-130">notApplicable</span></span>|<span data-ttu-id="86da0-131">-1</span><span class="sxs-lookup"><span data-stu-id="86da0-131">-1</span></span>|<span data-ttu-id="86da0-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="86da0-132">The application is not applicable.</span></span>|





