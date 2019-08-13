---
title: androidDeviceOwnerPlayStoreMode 枚举类型
description: Android 设备所有者播放存储模式类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d883091a7162c7cb0da40113430edbdc66a9cfa7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334806"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="b770b-103">androidDeviceOwnerPlayStoreMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b770b-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="b770b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b770b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b770b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b770b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b770b-106">Android 设备所有者播放存储模式类型。</span><span class="sxs-lookup"><span data-stu-id="b770b-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="b770b-107">成员</span><span class="sxs-lookup"><span data-stu-id="b770b-107">Members</span></span>
|<span data-ttu-id="b770b-108">成员</span><span class="sxs-lookup"><span data-stu-id="b770b-108">Member</span></span>|<span data-ttu-id="b770b-109">值</span><span class="sxs-lookup"><span data-stu-id="b770b-109">Value</span></span>|<span data-ttu-id="b770b-110">说明</span><span class="sxs-lookup"><span data-stu-id="b770b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b770b-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b770b-111">notConfigured</span></span>|<span data-ttu-id="b770b-112">0</span><span class="sxs-lookup"><span data-stu-id="b770b-112">0</span></span>|<span data-ttu-id="b770b-113">未配置</span><span class="sxs-lookup"><span data-stu-id="b770b-113">Not Configured</span></span>|
|<span data-ttu-id="b770b-114">allowList</span><span class="sxs-lookup"><span data-stu-id="b770b-114">allowList</span></span>|<span data-ttu-id="b770b-115">1</span><span class="sxs-lookup"><span data-stu-id="b770b-115">1</span></span>|<span data-ttu-id="b770b-116">只有策略中的应用程序可用, 并且不在该策略中的任何应用程序将自动从设备中卸载。</span><span class="sxs-lookup"><span data-stu-id="b770b-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="b770b-117">阻止列表</span><span class="sxs-lookup"><span data-stu-id="b770b-117">blockList</span></span>|<span data-ttu-id="b770b-118">双面</span><span class="sxs-lookup"><span data-stu-id="b770b-118">2</span></span>|<span data-ttu-id="b770b-119">所有应用均可用, 并且任何不应在设备上的应用程序应在应用程序策略中显式标记为 "已阻止"。</span><span class="sxs-lookup"><span data-stu-id="b770b-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



