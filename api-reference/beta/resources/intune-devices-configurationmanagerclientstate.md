---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 36abbe4451a6e053387b27fce3e9a4e25dcc1a95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806249"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="1e176-103">configurationManagerClientState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1e176-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="1e176-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1e176-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e176-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e176-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e176-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e176-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e176-107">配置管理器客户端状态</span><span class="sxs-lookup"><span data-stu-id="1e176-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="1e176-108">成员</span><span class="sxs-lookup"><span data-stu-id="1e176-108">Members</span></span>
|<span data-ttu-id="1e176-109">成员</span><span class="sxs-lookup"><span data-stu-id="1e176-109">Member</span></span>|<span data-ttu-id="1e176-110">值</span><span class="sxs-lookup"><span data-stu-id="1e176-110">Value</span></span>|<span data-ttu-id="1e176-111">Description</span><span class="sxs-lookup"><span data-stu-id="1e176-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e176-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1e176-112">unknown</span></span>|<span data-ttu-id="1e176-113">0</span><span class="sxs-lookup"><span data-stu-id="1e176-113">0</span></span>|<span data-ttu-id="1e176-114">配置管理器代理早于 1806年或未安装或此设备超过 30 天未签入 Intune。</span><span class="sxs-lookup"><span data-stu-id="1e176-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="1e176-115">安装</span><span class="sxs-lookup"><span data-stu-id="1e176-115">installed</span></span>|<span data-ttu-id="1e176-116">1</span><span class="sxs-lookup"><span data-stu-id="1e176-116">1</span></span>|<span data-ttu-id="1e176-117">配置管理器代理已安装，但可能不出现在配置管理器控制台尚未。</span><span class="sxs-lookup"><span data-stu-id="1e176-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="1e176-118">等待几个小时才能刷新。</span><span class="sxs-lookup"><span data-stu-id="1e176-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="1e176-119">正常运行</span><span class="sxs-lookup"><span data-stu-id="1e176-119">healthy</span></span>|<span data-ttu-id="1e176-120">7</span><span class="sxs-lookup"><span data-stu-id="1e176-120">7</span></span>|<span data-ttu-id="1e176-121">此设备就能够成功签入的配置管理器服务。</span><span class="sxs-lookup"><span data-stu-id="1e176-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="1e176-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="1e176-122">installFailed</span></span>|<span data-ttu-id="1e176-123">8</span><span class="sxs-lookup"><span data-stu-id="1e176-123">8</span></span>|<span data-ttu-id="1e176-124">配置管理器代理安装失败。</span><span class="sxs-lookup"><span data-stu-id="1e176-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="1e176-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="1e176-125">updateFailed</span></span>|<span data-ttu-id="1e176-126">11</span><span class="sxs-lookup"><span data-stu-id="1e176-126">11</span></span>|<span data-ttu-id="1e176-127">从 x 版本到版本的配置管理器代理 y 的更新失败。</span><span class="sxs-lookup"><span data-stu-id="1e176-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="1e176-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="1e176-128">communicationError</span></span>|<span data-ttu-id="1e176-129">19</span><span class="sxs-lookup"><span data-stu-id="1e176-129">19</span></span>|<span data-ttu-id="1e176-130">配置管理器代理能够找到配置管理器服务在过去但现在不再能够。</span><span class="sxs-lookup"><span data-stu-id="1e176-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





