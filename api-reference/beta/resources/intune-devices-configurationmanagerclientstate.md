---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425783"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="5fb10-103">configurationManagerClientState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5fb10-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="5fb10-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5fb10-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5fb10-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5fb10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fb10-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fb10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fb10-107">配置管理器客户端状态</span><span class="sxs-lookup"><span data-stu-id="5fb10-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="5fb10-108">成员</span><span class="sxs-lookup"><span data-stu-id="5fb10-108">Members</span></span>
|<span data-ttu-id="5fb10-109">成员</span><span class="sxs-lookup"><span data-stu-id="5fb10-109">Member</span></span>|<span data-ttu-id="5fb10-110">值</span><span class="sxs-lookup"><span data-stu-id="5fb10-110">Value</span></span>|<span data-ttu-id="5fb10-111">说明</span><span class="sxs-lookup"><span data-stu-id="5fb10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb10-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5fb10-112">unknown</span></span>|<span data-ttu-id="5fb10-113">0</span><span class="sxs-lookup"><span data-stu-id="5fb10-113">0</span></span>|<span data-ttu-id="5fb10-114">配置管理器代理早于 1806年或未安装或此设备超过 30 天未签入 Intune。</span><span class="sxs-lookup"><span data-stu-id="5fb10-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="5fb10-115">安装</span><span class="sxs-lookup"><span data-stu-id="5fb10-115">installed</span></span>|<span data-ttu-id="5fb10-116">1</span><span class="sxs-lookup"><span data-stu-id="5fb10-116">1</span></span>|<span data-ttu-id="5fb10-117">配置管理器代理已安装，但可能不出现在配置管理器控制台尚未。</span><span class="sxs-lookup"><span data-stu-id="5fb10-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="5fb10-118">等待几个小时才能刷新。</span><span class="sxs-lookup"><span data-stu-id="5fb10-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="5fb10-119">正常运行</span><span class="sxs-lookup"><span data-stu-id="5fb10-119">healthy</span></span>|<span data-ttu-id="5fb10-120">7</span><span class="sxs-lookup"><span data-stu-id="5fb10-120">7</span></span>|<span data-ttu-id="5fb10-121">此设备就能够成功签入的配置管理器服务。</span><span class="sxs-lookup"><span data-stu-id="5fb10-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="5fb10-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="5fb10-122">installFailed</span></span>|<span data-ttu-id="5fb10-123">8</span><span class="sxs-lookup"><span data-stu-id="5fb10-123">8</span></span>|<span data-ttu-id="5fb10-124">配置管理器代理安装失败。</span><span class="sxs-lookup"><span data-stu-id="5fb10-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="5fb10-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="5fb10-125">updateFailed</span></span>|<span data-ttu-id="5fb10-126">11</span><span class="sxs-lookup"><span data-stu-id="5fb10-126">11</span></span>|<span data-ttu-id="5fb10-127">从 x 版本到版本的配置管理器代理 y 的更新失败。</span><span class="sxs-lookup"><span data-stu-id="5fb10-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="5fb10-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="5fb10-128">communicationError</span></span>|<span data-ttu-id="5fb10-129">19</span><span class="sxs-lookup"><span data-stu-id="5fb10-129">19</span></span>|<span data-ttu-id="5fb10-130">配置管理器代理能够找到配置管理器服务在过去但现在不再能够。</span><span class="sxs-lookup"><span data-stu-id="5fb10-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




