---
title: androidDeviceOwnerPlayStoreMode 枚举类型
description: Android 设备所有者播放存储模式类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00909f739773e67d4b5a1ae87f53982b627f511e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556391"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="81612-103">androidDeviceOwnerPlayStoreMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="81612-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="81612-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81612-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81612-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81612-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81612-106">Android 设备所有者播放存储模式类型。</span><span class="sxs-lookup"><span data-stu-id="81612-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="81612-107">成员</span><span class="sxs-lookup"><span data-stu-id="81612-107">Members</span></span>
|<span data-ttu-id="81612-108">成员</span><span class="sxs-lookup"><span data-stu-id="81612-108">Member</span></span>|<span data-ttu-id="81612-109">值</span><span class="sxs-lookup"><span data-stu-id="81612-109">Value</span></span>|<span data-ttu-id="81612-110">说明</span><span class="sxs-lookup"><span data-stu-id="81612-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81612-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="81612-111">notConfigured</span></span>|<span data-ttu-id="81612-112">0</span><span class="sxs-lookup"><span data-stu-id="81612-112">0</span></span>|<span data-ttu-id="81612-113">未配置</span><span class="sxs-lookup"><span data-stu-id="81612-113">Not Configured</span></span>|
|<span data-ttu-id="81612-114">allowList</span><span class="sxs-lookup"><span data-stu-id="81612-114">allowList</span></span>|<span data-ttu-id="81612-115">1</span><span class="sxs-lookup"><span data-stu-id="81612-115">1</span></span>|<span data-ttu-id="81612-116">只有策略中的应用程序可用, 并且不在该策略中的任何应用程序将自动从设备中卸载。</span><span class="sxs-lookup"><span data-stu-id="81612-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="81612-117">阻止列表</span><span class="sxs-lookup"><span data-stu-id="81612-117">blockList</span></span>|<span data-ttu-id="81612-118">2 </span><span class="sxs-lookup"><span data-stu-id="81612-118">2</span></span>|<span data-ttu-id="81612-119">所有应用均可用, 并且任何不应在设备上的应用程序应在应用程序策略中显式标记为 "已阻止"。</span><span class="sxs-lookup"><span data-stu-id="81612-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|





