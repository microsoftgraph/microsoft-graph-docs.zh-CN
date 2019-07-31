---
title: windowsSModeConfiguration 枚举类型
description: 配置 S 模式解锁的可能选项
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 30e130a0d482e7334d9a8fb1fc01601ad0094822
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968741"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="141e0-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="141e0-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="141e0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="141e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="141e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="141e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="141e0-106">配置 S 模式解锁的可能选项</span><span class="sxs-lookup"><span data-stu-id="141e0-106">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="141e0-107">成员</span><span class="sxs-lookup"><span data-stu-id="141e0-107">Members</span></span>
|<span data-ttu-id="141e0-108">成员</span><span class="sxs-lookup"><span data-stu-id="141e0-108">Member</span></span>|<span data-ttu-id="141e0-109">值</span><span class="sxs-lookup"><span data-stu-id="141e0-109">Value</span></span>|<span data-ttu-id="141e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="141e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="141e0-111">noRestriction</span><span class="sxs-lookup"><span data-stu-id="141e0-111">noRestriction</span></span>|<span data-ttu-id="141e0-112">0</span><span class="sxs-lookup"><span data-stu-id="141e0-112">0</span></span>|<span data-ttu-id="141e0-113">此选项将删除对解锁 S 模式的所有限制-默认</span><span class="sxs-lookup"><span data-stu-id="141e0-113">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="141e0-114">数据</span><span class="sxs-lookup"><span data-stu-id="141e0-114">block</span></span>|<span data-ttu-id="141e0-115">1</span><span class="sxs-lookup"><span data-stu-id="141e0-115">1</span></span>|<span data-ttu-id="141e0-116">此选项将阻止用户从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="141e0-116">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="141e0-117">解锁</span><span class="sxs-lookup"><span data-stu-id="141e0-117">unlock</span></span>|<span data-ttu-id="141e0-118">双面</span><span class="sxs-lookup"><span data-stu-id="141e0-118">2</span></span>|<span data-ttu-id="141e0-119">此选项将从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="141e0-119">This option will unlock the device from S mode</span></span>|





