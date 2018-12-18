---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: tfitzmac
ms.openlocfilehash: dc67a5fb1c517e65da937996ed65adaa621fa3c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354045"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="8b82d-103">configurationManagerClientState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8b82d-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="8b82d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8b82d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b82d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b82d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b82d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8b82d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b82d-107">配置管理器客户端状态</span><span class="sxs-lookup"><span data-stu-id="8b82d-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="8b82d-108">成员</span><span class="sxs-lookup"><span data-stu-id="8b82d-108">Members</span></span>
|<span data-ttu-id="8b82d-109">成员</span><span class="sxs-lookup"><span data-stu-id="8b82d-109">Member</span></span>|<span data-ttu-id="8b82d-110">值</span><span class="sxs-lookup"><span data-stu-id="8b82d-110">Value</span></span>|<span data-ttu-id="8b82d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8b82d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b82d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="8b82d-112">unknown</span></span>|<span data-ttu-id="8b82d-113">0</span><span class="sxs-lookup"><span data-stu-id="8b82d-113">0</span></span>|<span data-ttu-id="8b82d-114">配置管理器代理早于 1806年或未安装或此设备超过 30 天未签入 Intune。</span><span class="sxs-lookup"><span data-stu-id="8b82d-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="8b82d-115">安装</span><span class="sxs-lookup"><span data-stu-id="8b82d-115">installed</span></span>|<span data-ttu-id="8b82d-116">1</span><span class="sxs-lookup"><span data-stu-id="8b82d-116">1</span></span>|<span data-ttu-id="8b82d-117">配置管理器代理已安装，但可能不出现在配置管理器控制台尚未。</span><span class="sxs-lookup"><span data-stu-id="8b82d-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="8b82d-118">等待几个小时才能刷新。</span><span class="sxs-lookup"><span data-stu-id="8b82d-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="8b82d-119">正常运行</span><span class="sxs-lookup"><span data-stu-id="8b82d-119">healthy</span></span>|<span data-ttu-id="8b82d-120">7</span><span class="sxs-lookup"><span data-stu-id="8b82d-120">7</span></span>|<span data-ttu-id="8b82d-121">此设备就能够成功签入的配置管理器服务。</span><span class="sxs-lookup"><span data-stu-id="8b82d-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="8b82d-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="8b82d-122">installFailed</span></span>|<span data-ttu-id="8b82d-123">8</span><span class="sxs-lookup"><span data-stu-id="8b82d-123">8</span></span>|<span data-ttu-id="8b82d-124">配置管理器代理安装失败。</span><span class="sxs-lookup"><span data-stu-id="8b82d-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="8b82d-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="8b82d-125">updateFailed</span></span>|<span data-ttu-id="8b82d-126">11</span><span class="sxs-lookup"><span data-stu-id="8b82d-126">11</span></span>|<span data-ttu-id="8b82d-127">从 x 版本到版本的配置管理器代理 y 的更新失败。</span><span class="sxs-lookup"><span data-stu-id="8b82d-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="8b82d-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="8b82d-128">communicationError</span></span>|<span data-ttu-id="8b82d-129">19</span><span class="sxs-lookup"><span data-stu-id="8b82d-129">19</span></span>|<span data-ttu-id="8b82d-130">配置管理器代理能够找到配置管理器服务在过去但现在不再能够。</span><span class="sxs-lookup"><span data-stu-id="8b82d-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





