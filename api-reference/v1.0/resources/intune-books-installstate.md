---
title: installState 枚举类型
description: 安装状态的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b50fb44c2af31efff81f2dd7097505f71bc791d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947546"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="7d560-103">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7d560-103">installState enum type</span></span>

> <span data-ttu-id="7d560-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d560-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d560-105">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="7d560-105">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="7d560-106">成员</span><span class="sxs-lookup"><span data-stu-id="7d560-106">Members</span></span>
|<span data-ttu-id="7d560-107">成员</span><span class="sxs-lookup"><span data-stu-id="7d560-107">Member</span></span>|<span data-ttu-id="7d560-108">值</span><span class="sxs-lookup"><span data-stu-id="7d560-108">Value</span></span>|<span data-ttu-id="7d560-109">说明</span><span class="sxs-lookup"><span data-stu-id="7d560-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d560-110">notApplicable</span><span class="sxs-lookup"><span data-stu-id="7d560-110">notApplicable</span></span>|<span data-ttu-id="7d560-111">0</span><span class="sxs-lookup"><span data-stu-id="7d560-111">0</span></span>|<span data-ttu-id="7d560-112">不适用。</span><span class="sxs-lookup"><span data-stu-id="7d560-112">Not Applicable.</span></span>|
|<span data-ttu-id="7d560-113">安装</span><span class="sxs-lookup"><span data-stu-id="7d560-113">installed</span></span>|<span data-ttu-id="7d560-114">1</span><span class="sxs-lookup"><span data-stu-id="7d560-114">1</span></span>|<span data-ttu-id="7d560-115">安装。</span><span class="sxs-lookup"><span data-stu-id="7d560-115">Installed.</span></span>|
|<span data-ttu-id="7d560-116">failed</span><span class="sxs-lookup"><span data-stu-id="7d560-116">failed</span></span>|<span data-ttu-id="7d560-117">2</span><span class="sxs-lookup"><span data-stu-id="7d560-117">2</span></span>|<span data-ttu-id="7d560-118">失败。</span><span class="sxs-lookup"><span data-stu-id="7d560-118">Failed.</span></span>|
|<span data-ttu-id="7d560-119">notInstalled</span><span class="sxs-lookup"><span data-stu-id="7d560-119">notInstalled</span></span>|<span data-ttu-id="7d560-120">3</span><span class="sxs-lookup"><span data-stu-id="7d560-120">3</span></span>|<span data-ttu-id="7d560-121">未安装。</span><span class="sxs-lookup"><span data-stu-id="7d560-121">Not Installed.</span></span>|
|<span data-ttu-id="7d560-122">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="7d560-122">uninstallFailed</span></span>|<span data-ttu-id="7d560-123">4</span><span class="sxs-lookup"><span data-stu-id="7d560-123">4</span></span>|<span data-ttu-id="7d560-124">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="7d560-124">Uninstall Failed.</span></span>|
|<span data-ttu-id="7d560-125">unknown</span><span class="sxs-lookup"><span data-stu-id="7d560-125">unknown</span></span>|<span data-ttu-id="7d560-126">5</span><span class="sxs-lookup"><span data-stu-id="7d560-126">5</span></span>|<span data-ttu-id="7d560-127">未知。</span><span class="sxs-lookup"><span data-stu-id="7d560-127">Unknown.</span></span>|



