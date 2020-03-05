---
title: androidDeviceOwnerPlayStoreMode 枚举类型
description: Android 设备所有者播放存储模式类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 32eb96d5429380eaa6d9f4ffe021d37c62f3fffa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486477"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="c115c-103">androidDeviceOwnerPlayStoreMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c115c-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="c115c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c115c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c115c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c115c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c115c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c115c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c115c-107">Android 设备所有者播放存储模式类型。</span><span class="sxs-lookup"><span data-stu-id="c115c-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="c115c-108">成员</span><span class="sxs-lookup"><span data-stu-id="c115c-108">Members</span></span>
|<span data-ttu-id="c115c-109">成员</span><span class="sxs-lookup"><span data-stu-id="c115c-109">Member</span></span>|<span data-ttu-id="c115c-110">值</span><span class="sxs-lookup"><span data-stu-id="c115c-110">Value</span></span>|<span data-ttu-id="c115c-111">说明</span><span class="sxs-lookup"><span data-stu-id="c115c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c115c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c115c-112">notConfigured</span></span>|<span data-ttu-id="c115c-113">0</span><span class="sxs-lookup"><span data-stu-id="c115c-113">0</span></span>|<span data-ttu-id="c115c-114">未配置</span><span class="sxs-lookup"><span data-stu-id="c115c-114">Not Configured</span></span>|
|<span data-ttu-id="c115c-115">allowList</span><span class="sxs-lookup"><span data-stu-id="c115c-115">allowList</span></span>|<span data-ttu-id="c115c-116">1 </span><span class="sxs-lookup"><span data-stu-id="c115c-116">1</span></span>|<span data-ttu-id="c115c-117">只有策略中的应用程序可用，并且不在该策略中的任何应用程序将自动从设备中卸载。</span><span class="sxs-lookup"><span data-stu-id="c115c-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="c115c-118">阻止列表</span><span class="sxs-lookup"><span data-stu-id="c115c-118">blockList</span></span>|<span data-ttu-id="c115c-119">2 </span><span class="sxs-lookup"><span data-stu-id="c115c-119">2</span></span>|<span data-ttu-id="c115c-120">所有应用均可用，并且任何不应在设备上的应用程序应在应用程序策略中显式标记为 "已阻止"。</span><span class="sxs-lookup"><span data-stu-id="c115c-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



