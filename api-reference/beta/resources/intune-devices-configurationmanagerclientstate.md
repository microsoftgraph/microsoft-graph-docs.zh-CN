---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: de8f2af7c6d35b28154f00a4eac3bb20a4bdf64d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690229"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="24dda-103">configurationManagerClientState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="24dda-103">configurationManagerClientState enum type</span></span>

<span data-ttu-id="24dda-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24dda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24dda-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24dda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24dda-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24dda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24dda-107">配置管理器客户端状态</span><span class="sxs-lookup"><span data-stu-id="24dda-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="24dda-108">成员</span><span class="sxs-lookup"><span data-stu-id="24dda-108">Members</span></span>
|<span data-ttu-id="24dda-109">成员</span><span class="sxs-lookup"><span data-stu-id="24dda-109">Member</span></span>|<span data-ttu-id="24dda-110">值</span><span class="sxs-lookup"><span data-stu-id="24dda-110">Value</span></span>|<span data-ttu-id="24dda-111">说明</span><span class="sxs-lookup"><span data-stu-id="24dda-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24dda-112">unknown</span><span class="sxs-lookup"><span data-stu-id="24dda-112">unknown</span></span>|<span data-ttu-id="24dda-113">0</span><span class="sxs-lookup"><span data-stu-id="24dda-113">0</span></span>|<span data-ttu-id="24dda-114">配置管理器代理早于1806或未安装，或者此设备未签入 Intune 的30天。</span><span class="sxs-lookup"><span data-stu-id="24dda-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="24dda-115">了</span><span class="sxs-lookup"><span data-stu-id="24dda-115">installed</span></span>|<span data-ttu-id="24dda-116">1</span><span class="sxs-lookup"><span data-stu-id="24dda-116">1</span></span>|<span data-ttu-id="24dda-117">配置管理器代理已安装，但可能尚未在 configuration manager 控制台中显示。</span><span class="sxs-lookup"><span data-stu-id="24dda-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="24dda-118">请等待几小时，让其刷新。</span><span class="sxs-lookup"><span data-stu-id="24dda-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="24dda-119">运转</span><span class="sxs-lookup"><span data-stu-id="24dda-119">healthy</span></span>|<span data-ttu-id="24dda-120">7 </span><span class="sxs-lookup"><span data-stu-id="24dda-120">7</span></span>|<span data-ttu-id="24dda-121">此设备能够成功签入 configuration manager 服务。</span><span class="sxs-lookup"><span data-stu-id="24dda-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="24dda-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="24dda-122">installFailed</span></span>|<span data-ttu-id="24dda-123">8 </span><span class="sxs-lookup"><span data-stu-id="24dda-123">8</span></span>|<span data-ttu-id="24dda-124">配置管理器代理安装失败。</span><span class="sxs-lookup"><span data-stu-id="24dda-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="24dda-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="24dda-125">updateFailed</span></span>|<span data-ttu-id="24dda-126">11x17</span><span class="sxs-lookup"><span data-stu-id="24dda-126">11</span></span>|<span data-ttu-id="24dda-127">从版本 x 更新到配置管理器代理版本 y 的更新失败。</span><span class="sxs-lookup"><span data-stu-id="24dda-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="24dda-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="24dda-128">communicationError</span></span>|<span data-ttu-id="24dda-129">合</span><span class="sxs-lookup"><span data-stu-id="24dda-129">19</span></span>|<span data-ttu-id="24dda-130">Configuration manager 代理在过去能够到达 configuration manager 服务，但现在无法再访问。</span><span class="sxs-lookup"><span data-stu-id="24dda-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





