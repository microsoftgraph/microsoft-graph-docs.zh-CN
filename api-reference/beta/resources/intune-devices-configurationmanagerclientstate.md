---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba7de7ee3612c4d1e8e419522e8d18587339343c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370282"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="ba0b4-103">configurationManagerClientState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ba0b4-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="ba0b4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba0b4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba0b4-106">配置管理器客户端状态</span><span class="sxs-lookup"><span data-stu-id="ba0b4-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="ba0b4-107">成员</span><span class="sxs-lookup"><span data-stu-id="ba0b4-107">Members</span></span>
|<span data-ttu-id="ba0b4-108">成员</span><span class="sxs-lookup"><span data-stu-id="ba0b4-108">Member</span></span>|<span data-ttu-id="ba0b4-109">值</span><span class="sxs-lookup"><span data-stu-id="ba0b4-109">Value</span></span>|<span data-ttu-id="ba0b4-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba0b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba0b4-111">unknown</span><span class="sxs-lookup"><span data-stu-id="ba0b4-111">unknown</span></span>|<span data-ttu-id="ba0b4-112">0</span><span class="sxs-lookup"><span data-stu-id="ba0b4-112">0</span></span>|<span data-ttu-id="ba0b4-113">配置管理器代理早于1806或未安装, 或者此设备未签入 Intune 的30天。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="ba0b4-114">了</span><span class="sxs-lookup"><span data-stu-id="ba0b4-114">installed</span></span>|<span data-ttu-id="ba0b4-115">1</span><span class="sxs-lookup"><span data-stu-id="ba0b4-115">1</span></span>|<span data-ttu-id="ba0b4-116">配置管理器代理已安装, 但可能尚未在 configuration manager 控制台中显示。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="ba0b4-117">请等待几小时, 让其刷新。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="ba0b4-118">运转</span><span class="sxs-lookup"><span data-stu-id="ba0b4-118">healthy</span></span>|<span data-ttu-id="ba0b4-119">步</span><span class="sxs-lookup"><span data-stu-id="ba0b4-119">7</span></span>|<span data-ttu-id="ba0b4-120">此设备能够成功签入 configuration manager 服务。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="ba0b4-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="ba0b4-121">installFailed</span></span>|<span data-ttu-id="ba0b4-122">utf-8</span><span class="sxs-lookup"><span data-stu-id="ba0b4-122">8</span></span>|<span data-ttu-id="ba0b4-123">配置管理器代理安装失败。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="ba0b4-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="ba0b4-124">updateFailed</span></span>|<span data-ttu-id="ba0b4-125">11x17</span><span class="sxs-lookup"><span data-stu-id="ba0b4-125">11</span></span>|<span data-ttu-id="ba0b4-126">从版本 x 更新到配置管理器代理版本 y 的更新失败。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="ba0b4-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="ba0b4-127">communicationError</span></span>|<span data-ttu-id="ba0b4-128">合</span><span class="sxs-lookup"><span data-stu-id="ba0b4-128">19</span></span>|<span data-ttu-id="ba0b4-129">Configuration manager 代理在过去能够到达 configuration manager 服务, 但现在无法再访问。</span><span class="sxs-lookup"><span data-stu-id="ba0b4-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |



