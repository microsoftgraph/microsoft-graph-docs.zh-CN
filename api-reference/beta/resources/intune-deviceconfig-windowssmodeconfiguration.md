---
title: windowsSModeConfiguration 枚举类型
description: 配置 S 模式解锁的可能选项
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd9b4c696c7456e4cf926764bfadde3fbd591a6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525402"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="b6606-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b6606-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="b6606-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b6606-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6606-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6606-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6606-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6606-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6606-107">配置 S 模式解锁的可能选项</span><span class="sxs-lookup"><span data-stu-id="b6606-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="b6606-108">成员</span><span class="sxs-lookup"><span data-stu-id="b6606-108">Members</span></span>
|<span data-ttu-id="b6606-109">成员</span><span class="sxs-lookup"><span data-stu-id="b6606-109">Member</span></span>|<span data-ttu-id="b6606-110">值</span><span class="sxs-lookup"><span data-stu-id="b6606-110">Value</span></span>|<span data-ttu-id="b6606-111">说明</span><span class="sxs-lookup"><span data-stu-id="b6606-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6606-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="b6606-112">noRestriction</span></span>|<span data-ttu-id="b6606-113">0</span><span class="sxs-lookup"><span data-stu-id="b6606-113">0</span></span>|<span data-ttu-id="b6606-114">此选项将删除对解锁 S 模式的所有限制-默认</span><span class="sxs-lookup"><span data-stu-id="b6606-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="b6606-115">数据</span><span class="sxs-lookup"><span data-stu-id="b6606-115">block</span></span>|<span data-ttu-id="b6606-116">1 </span><span class="sxs-lookup"><span data-stu-id="b6606-116">1</span></span>|<span data-ttu-id="b6606-117">此选项将阻止用户从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="b6606-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="b6606-118">解锁</span><span class="sxs-lookup"><span data-stu-id="b6606-118">unlock</span></span>|<span data-ttu-id="b6606-119">2 </span><span class="sxs-lookup"><span data-stu-id="b6606-119">2</span></span>|<span data-ttu-id="b6606-120">此选项将从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="b6606-120">This option will unlock the device from S mode</span></span>|



