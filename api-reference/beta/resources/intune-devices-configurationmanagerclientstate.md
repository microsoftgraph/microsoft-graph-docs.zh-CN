---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6231ecebf407172f2c7178a130d90200868292
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776519"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="867d8-103">configurationManagerClientState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="867d8-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="867d8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="867d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="867d8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="867d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="867d8-106">配置管理器客户端状态</span><span class="sxs-lookup"><span data-stu-id="867d8-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="867d8-107">成员</span><span class="sxs-lookup"><span data-stu-id="867d8-107">Members</span></span>
|<span data-ttu-id="867d8-108">成员</span><span class="sxs-lookup"><span data-stu-id="867d8-108">Member</span></span>|<span data-ttu-id="867d8-109">值</span><span class="sxs-lookup"><span data-stu-id="867d8-109">Value</span></span>|<span data-ttu-id="867d8-110">说明</span><span class="sxs-lookup"><span data-stu-id="867d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="867d8-111">unknown</span><span class="sxs-lookup"><span data-stu-id="867d8-111">unknown</span></span>|<span data-ttu-id="867d8-112">0</span><span class="sxs-lookup"><span data-stu-id="867d8-112">0</span></span>|<span data-ttu-id="867d8-113">配置管理器代理早于1806或未安装, 或者此设备未签入 Intune 的30天。</span><span class="sxs-lookup"><span data-stu-id="867d8-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="867d8-114">了</span><span class="sxs-lookup"><span data-stu-id="867d8-114">installed</span></span>|<span data-ttu-id="867d8-115">1</span><span class="sxs-lookup"><span data-stu-id="867d8-115">1</span></span>|<span data-ttu-id="867d8-116">配置管理器代理已安装, 但可能尚未在 configuration manager 控制台中显示。</span><span class="sxs-lookup"><span data-stu-id="867d8-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="867d8-117">请等待几小时, 让其刷新。</span><span class="sxs-lookup"><span data-stu-id="867d8-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="867d8-118">运转</span><span class="sxs-lookup"><span data-stu-id="867d8-118">healthy</span></span>|<span data-ttu-id="867d8-119">步</span><span class="sxs-lookup"><span data-stu-id="867d8-119">7</span></span>|<span data-ttu-id="867d8-120">此设备能够成功签入 configuration manager 服务。</span><span class="sxs-lookup"><span data-stu-id="867d8-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="867d8-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="867d8-121">installFailed</span></span>|<span data-ttu-id="867d8-122">utf-8</span><span class="sxs-lookup"><span data-stu-id="867d8-122">8</span></span>|<span data-ttu-id="867d8-123">配置管理器代理安装失败。</span><span class="sxs-lookup"><span data-stu-id="867d8-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="867d8-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="867d8-124">updateFailed</span></span>|<span data-ttu-id="867d8-125">11x17</span><span class="sxs-lookup"><span data-stu-id="867d8-125">11</span></span>|<span data-ttu-id="867d8-126">从版本 x 更新到配置管理器代理版本 y 的更新失败。</span><span class="sxs-lookup"><span data-stu-id="867d8-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="867d8-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="867d8-127">communicationError</span></span>|<span data-ttu-id="867d8-128">合</span><span class="sxs-lookup"><span data-stu-id="867d8-128">19</span></span>|<span data-ttu-id="867d8-129">configuration manager 代理在过去能够到达 configuration manager 服务, 但现在无法再访问。</span><span class="sxs-lookup"><span data-stu-id="867d8-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





