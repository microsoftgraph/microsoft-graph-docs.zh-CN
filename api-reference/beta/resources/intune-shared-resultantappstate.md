---
title: resultantAppState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5e39426c26f819a73d933c47a296378021d62b2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084098"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="51b64-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="51b64-103">resultantAppState enum type</span></span>

<span data-ttu-id="51b64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51b64-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51b64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51b64-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51b64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51b64-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51b64-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="51b64-108">成员</span><span class="sxs-lookup"><span data-stu-id="51b64-108">Members</span></span>
|<span data-ttu-id="51b64-109">成员</span><span class="sxs-lookup"><span data-stu-id="51b64-109">Member</span></span>|<span data-ttu-id="51b64-110">值</span><span class="sxs-lookup"><span data-stu-id="51b64-110">Value</span></span>|<span data-ttu-id="51b64-111">说明</span><span class="sxs-lookup"><span data-stu-id="51b64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b64-112">了</span><span class="sxs-lookup"><span data-stu-id="51b64-112">installed</span></span>|<span data-ttu-id="51b64-113">1 </span><span class="sxs-lookup"><span data-stu-id="51b64-113">1</span></span>|<span data-ttu-id="51b64-114">安装应用程序时没有出现任何错误</span><span class="sxs-lookup"><span data-stu-id="51b64-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="51b64-115">未能</span><span class="sxs-lookup"><span data-stu-id="51b64-115">failed</span></span>|<span data-ttu-id="51b64-116">2 </span><span class="sxs-lookup"><span data-stu-id="51b64-116">2</span></span>|<span data-ttu-id="51b64-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="51b64-117">The application failed to install.</span></span>|
|<span data-ttu-id="51b64-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="51b64-118">notInstalled</span></span>|<span data-ttu-id="51b64-119">第三章</span><span class="sxs-lookup"><span data-stu-id="51b64-119">3</span></span>|<span data-ttu-id="51b64-120">未安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="51b64-120">The application is not installed.</span></span>|
|<span data-ttu-id="51b64-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="51b64-121">uninstallFailed</span></span>|<span data-ttu-id="51b64-122">4 </span><span class="sxs-lookup"><span data-stu-id="51b64-122">4</span></span>|<span data-ttu-id="51b64-123">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="51b64-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="51b64-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="51b64-124">pendingInstall</span></span>|<span data-ttu-id="51b64-125">5 </span><span class="sxs-lookup"><span data-stu-id="51b64-125">5</span></span>|<span data-ttu-id="51b64-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="51b64-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="51b64-127">unknown</span><span class="sxs-lookup"><span data-stu-id="51b64-127">unknown</span></span>|<span data-ttu-id="51b64-128">99</span><span class="sxs-lookup"><span data-stu-id="51b64-128">99</span></span>|<span data-ttu-id="51b64-129">应用程序的状态未知。</span><span class="sxs-lookup"><span data-stu-id="51b64-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="51b64-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="51b64-130">notApplicable</span></span>|<span data-ttu-id="51b64-131">-1</span><span class="sxs-lookup"><span data-stu-id="51b64-131">-1</span></span>|<span data-ttu-id="51b64-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="51b64-132">The application is not applicable.</span></span>|






