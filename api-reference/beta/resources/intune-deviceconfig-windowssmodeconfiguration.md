---
title: windowsSModeConfiguration 枚举类型
description: 配置 S 模式解锁的可能选项
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7dc2eb81f426ca5e8e708fa5b5cdc6904ed9cfa3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444017"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="b013c-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b013c-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="b013c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b013c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b013c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b013c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b013c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b013c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b013c-107">配置 S 模式解锁的可能选项</span><span class="sxs-lookup"><span data-stu-id="b013c-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="b013c-108">成员</span><span class="sxs-lookup"><span data-stu-id="b013c-108">Members</span></span>
|<span data-ttu-id="b013c-109">成员</span><span class="sxs-lookup"><span data-stu-id="b013c-109">Member</span></span>|<span data-ttu-id="b013c-110">值</span><span class="sxs-lookup"><span data-stu-id="b013c-110">Value</span></span>|<span data-ttu-id="b013c-111">说明</span><span class="sxs-lookup"><span data-stu-id="b013c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b013c-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="b013c-112">noRestriction</span></span>|<span data-ttu-id="b013c-113">0</span><span class="sxs-lookup"><span data-stu-id="b013c-113">0</span></span>|<span data-ttu-id="b013c-114">此选项将删除对解锁 S 模式的所有限制-默认</span><span class="sxs-lookup"><span data-stu-id="b013c-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="b013c-115">数据</span><span class="sxs-lookup"><span data-stu-id="b013c-115">block</span></span>|<span data-ttu-id="b013c-116">1</span><span class="sxs-lookup"><span data-stu-id="b013c-116">1</span></span>|<span data-ttu-id="b013c-117">此选项将阻止用户从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="b013c-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="b013c-118">解锁</span><span class="sxs-lookup"><span data-stu-id="b013c-118">unlock</span></span>|<span data-ttu-id="b013c-119">双面</span><span class="sxs-lookup"><span data-stu-id="b013c-119">2</span></span>|<span data-ttu-id="b013c-120">此选项将从 S 模式解锁设备</span><span class="sxs-lookup"><span data-stu-id="b013c-120">This option will unlock the device from S mode</span></span>|



