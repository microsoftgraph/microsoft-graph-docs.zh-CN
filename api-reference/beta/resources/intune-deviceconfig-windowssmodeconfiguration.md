---
title: windowsSModeConfiguration 枚举类型
description: 配置 S 模式解锁的可能选项
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 467879cf7992a60203164d5db6f7e657a77f87d4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943814"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="eaebf-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="eaebf-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="eaebf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eaebf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaebf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eaebf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaebf-106">配置 S 模式解锁的可能选项</span><span class="sxs-lookup"><span data-stu-id="eaebf-106">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="eaebf-107">成员</span><span class="sxs-lookup"><span data-stu-id="eaebf-107">Members</span></span>
|<span data-ttu-id="eaebf-108">成员</span><span class="sxs-lookup"><span data-stu-id="eaebf-108">Member</span></span>|<span data-ttu-id="eaebf-109">值</span><span class="sxs-lookup"><span data-stu-id="eaebf-109">Value</span></span>|<span data-ttu-id="eaebf-110">说明</span><span class="sxs-lookup"><span data-stu-id="eaebf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaebf-111">noRestriction</span><span class="sxs-lookup"><span data-stu-id="eaebf-111">noRestriction</span></span>|<span data-ttu-id="eaebf-112">0</span><span class="sxs-lookup"><span data-stu-id="eaebf-112">0</span></span>|<span data-ttu-id="eaebf-113">此选项将删除对解锁 S 模式的所有限制-默认</span><span class="sxs-lookup"><span data-stu-id="eaebf-113">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="eaebf-114">数据</span><span class="sxs-lookup"><span data-stu-id="eaebf-114">block</span></span>|<span data-ttu-id="eaebf-115">1</span><span class="sxs-lookup"><span data-stu-id="eaebf-115">1</span></span>|<span data-ttu-id="eaebf-116">此选项将阻止用户从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="eaebf-116">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="eaebf-117">解锁</span><span class="sxs-lookup"><span data-stu-id="eaebf-117">unlock</span></span>|<span data-ttu-id="eaebf-118">双面</span><span class="sxs-lookup"><span data-stu-id="eaebf-118">2</span></span>|<span data-ttu-id="eaebf-119">此选项将从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="eaebf-119">This option will unlock the device from S mode</span></span>|




