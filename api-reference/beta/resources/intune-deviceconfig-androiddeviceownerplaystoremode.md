---
title: androidDeviceOwnerPlayStoreMode 枚举类型
description: Android 设备所有者播放存储模式类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 802775fc56a3c961e03e757ac710abca35d8c8f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968701"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="8dfc7-103">androidDeviceOwnerPlayStoreMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8dfc7-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="8dfc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dfc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dfc7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8dfc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dfc7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8dfc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dfc7-107">Android 设备所有者播放存储模式类型。</span><span class="sxs-lookup"><span data-stu-id="8dfc7-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="8dfc7-108">成员</span><span class="sxs-lookup"><span data-stu-id="8dfc7-108">Members</span></span>
|<span data-ttu-id="8dfc7-109">成员</span><span class="sxs-lookup"><span data-stu-id="8dfc7-109">Member</span></span>|<span data-ttu-id="8dfc7-110">值</span><span class="sxs-lookup"><span data-stu-id="8dfc7-110">Value</span></span>|<span data-ttu-id="8dfc7-111">说明</span><span class="sxs-lookup"><span data-stu-id="8dfc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dfc7-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8dfc7-112">notConfigured</span></span>|<span data-ttu-id="8dfc7-113">0</span><span class="sxs-lookup"><span data-stu-id="8dfc7-113">0</span></span>|<span data-ttu-id="8dfc7-114">未配置</span><span class="sxs-lookup"><span data-stu-id="8dfc7-114">Not Configured</span></span>|
|<span data-ttu-id="8dfc7-115">allowList</span><span class="sxs-lookup"><span data-stu-id="8dfc7-115">allowList</span></span>|<span data-ttu-id="8dfc7-116">1 </span><span class="sxs-lookup"><span data-stu-id="8dfc7-116">1</span></span>|<span data-ttu-id="8dfc7-117">只有策略中的应用程序可用，并且不在该策略中的任何应用程序将自动从设备中卸载。</span><span class="sxs-lookup"><span data-stu-id="8dfc7-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="8dfc7-118">阻止列表</span><span class="sxs-lookup"><span data-stu-id="8dfc7-118">blockList</span></span>|<span data-ttu-id="8dfc7-119">2 </span><span class="sxs-lookup"><span data-stu-id="8dfc7-119">2</span></span>|<span data-ttu-id="8dfc7-120">所有应用均可用，并且任何不应在设备上的应用程序应在应用程序策略中显式标记为 "已阻止"。</span><span class="sxs-lookup"><span data-stu-id="8dfc7-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|






