---
title: resultantAppState 枚举类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf3d7e8ef20b1458811ae1a49b23120f7cd153d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422682"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="9d9a5-103">resultantAppState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9d9a5-103">resultantAppState enum type</span></span>

> <span data-ttu-id="9d9a5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9d9a5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d9a5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d9a5-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9d9a5-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="9d9a5-108">成员</span><span class="sxs-lookup"><span data-stu-id="9d9a5-108">Members</span></span>
|<span data-ttu-id="9d9a5-109">成员</span><span class="sxs-lookup"><span data-stu-id="9d9a5-109">Member</span></span>|<span data-ttu-id="9d9a5-110">值</span><span class="sxs-lookup"><span data-stu-id="9d9a5-110">Value</span></span>|<span data-ttu-id="9d9a5-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d9a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d9a5-112">安装</span><span class="sxs-lookup"><span data-stu-id="9d9a5-112">installed</span></span>|<span data-ttu-id="9d9a5-113">1</span><span class="sxs-lookup"><span data-stu-id="9d9a5-113">1</span></span>|<span data-ttu-id="9d9a5-114">无错误安装应用程序</span><span class="sxs-lookup"><span data-stu-id="9d9a5-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="9d9a5-115">failed</span><span class="sxs-lookup"><span data-stu-id="9d9a5-115">failed</span></span>|<span data-ttu-id="9d9a5-116">2</span><span class="sxs-lookup"><span data-stu-id="9d9a5-116">2</span></span>|<span data-ttu-id="9d9a5-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-117">The application failed to install.</span></span>|
|<span data-ttu-id="9d9a5-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="9d9a5-118">notInstalled</span></span>|<span data-ttu-id="9d9a5-119">3</span><span class="sxs-lookup"><span data-stu-id="9d9a5-119">3</span></span>|<span data-ttu-id="9d9a5-120">不安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-120">The application is not installed.</span></span>|
|<span data-ttu-id="9d9a5-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="9d9a5-121">uninstallFailed</span></span>|<span data-ttu-id="9d9a5-122">4</span><span class="sxs-lookup"><span data-stu-id="9d9a5-122">4</span></span>|<span data-ttu-id="9d9a5-123">无法卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="9d9a5-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="9d9a5-124">pendingInstall</span></span>|<span data-ttu-id="9d9a5-125">5</span><span class="sxs-lookup"><span data-stu-id="9d9a5-125">5</span></span>|<span data-ttu-id="9d9a5-126">正在安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="9d9a5-127">unknown</span><span class="sxs-lookup"><span data-stu-id="9d9a5-127">unknown</span></span>|<span data-ttu-id="9d9a5-128">99</span><span class="sxs-lookup"><span data-stu-id="9d9a5-128">99</span></span>|<span data-ttu-id="9d9a5-129">未知的应用程序的状态。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="9d9a5-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="9d9a5-130">notApplicable</span></span>|<span data-ttu-id="9d9a5-131">-1</span><span class="sxs-lookup"><span data-stu-id="9d9a5-131">-1</span></span>|<span data-ttu-id="9d9a5-132">应用程序不适用。</span><span class="sxs-lookup"><span data-stu-id="9d9a5-132">The application is not applicable.</span></span>|




