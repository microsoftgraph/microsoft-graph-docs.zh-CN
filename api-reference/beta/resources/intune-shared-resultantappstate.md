---
title: resultantAppState 枚举类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 7b45353867abe77143fb97755aff457e0c81deb8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319423"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="21f7a-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21f7a-103">resultantAppState enum type</span></span>

> <span data-ttu-id="21f7a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="21f7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21f7a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21f7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21f7a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="21f7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21f7a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="21f7a-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="21f7a-108">成员</span><span class="sxs-lookup"><span data-stu-id="21f7a-108">Members</span></span>
|<span data-ttu-id="21f7a-109">成员</span><span class="sxs-lookup"><span data-stu-id="21f7a-109">Member</span></span>|<span data-ttu-id="21f7a-110">值</span><span class="sxs-lookup"><span data-stu-id="21f7a-110">Value</span></span>|<span data-ttu-id="21f7a-111">说明</span><span class="sxs-lookup"><span data-stu-id="21f7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21f7a-112">安装</span><span class="sxs-lookup"><span data-stu-id="21f7a-112">installed</span></span>|<span data-ttu-id="21f7a-113">1</span><span class="sxs-lookup"><span data-stu-id="21f7a-113">1</span></span>|<span data-ttu-id="21f7a-114">无错误安装应用程序</span><span class="sxs-lookup"><span data-stu-id="21f7a-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="21f7a-115">failed</span><span class="sxs-lookup"><span data-stu-id="21f7a-115">failed</span></span>|<span data-ttu-id="21f7a-116">2</span><span class="sxs-lookup"><span data-stu-id="21f7a-116">2</span></span>|<span data-ttu-id="21f7a-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="21f7a-117">The application failed to install.</span></span>|
|<span data-ttu-id="21f7a-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="21f7a-118">notInstalled</span></span>|<span data-ttu-id="21f7a-119">3</span><span class="sxs-lookup"><span data-stu-id="21f7a-119">3</span></span>|<span data-ttu-id="21f7a-120">不安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="21f7a-120">The application is not installed.</span></span>|
|<span data-ttu-id="21f7a-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="21f7a-121">uninstallFailed</span></span>|<span data-ttu-id="21f7a-122">4</span><span class="sxs-lookup"><span data-stu-id="21f7a-122">4</span></span>|<span data-ttu-id="21f7a-123">无法卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="21f7a-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="21f7a-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="21f7a-124">pendingInstall</span></span>|<span data-ttu-id="21f7a-125">5</span><span class="sxs-lookup"><span data-stu-id="21f7a-125">5</span></span>|<span data-ttu-id="21f7a-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="21f7a-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="21f7a-127">unknown</span><span class="sxs-lookup"><span data-stu-id="21f7a-127">unknown</span></span>|<span data-ttu-id="21f7a-128">99</span><span class="sxs-lookup"><span data-stu-id="21f7a-128">99</span></span>|<span data-ttu-id="21f7a-129">未知的应用程序的状态。</span><span class="sxs-lookup"><span data-stu-id="21f7a-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="21f7a-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="21f7a-130">notApplicable</span></span>|<span data-ttu-id="21f7a-131">-1</span><span class="sxs-lookup"><span data-stu-id="21f7a-131">-1</span></span>|<span data-ttu-id="21f7a-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="21f7a-132">The application is not applicable.</span></span>|





