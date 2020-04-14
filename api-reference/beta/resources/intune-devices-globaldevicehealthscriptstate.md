---
title: globalDeviceHealthScriptState 枚举类型
description: 指示是否启用全局设备运行状况脚本并将其状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e9b1ca70ca5c9d30d515b4d20bd27525249806fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470647"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="087b9-103">globalDeviceHealthScriptState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="087b9-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="087b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="087b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="087b9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="087b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="087b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="087b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="087b9-107">指示是否启用全局设备运行状况脚本并将其状态</span><span class="sxs-lookup"><span data-stu-id="087b9-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="087b9-108">成员</span><span class="sxs-lookup"><span data-stu-id="087b9-108">Members</span></span>
|<span data-ttu-id="087b9-109">成员</span><span class="sxs-lookup"><span data-stu-id="087b9-109">Member</span></span>|<span data-ttu-id="087b9-110">值</span><span class="sxs-lookup"><span data-stu-id="087b9-110">Value</span></span>|<span data-ttu-id="087b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="087b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="087b9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="087b9-112">notConfigured</span></span>|<span data-ttu-id="087b9-113">0</span><span class="sxs-lookup"><span data-stu-id="087b9-113">0</span></span>|<span data-ttu-id="087b9-114">未配置全局设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="087b9-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="087b9-115">决</span><span class="sxs-lookup"><span data-stu-id="087b9-115">pending</span></span>|<span data-ttu-id="087b9-116">1</span><span class="sxs-lookup"><span data-stu-id="087b9-116">1</span></span>|<span data-ttu-id="087b9-117">已配置全局设备运行状况脚本，但未完全启用</span><span class="sxs-lookup"><span data-stu-id="087b9-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="087b9-118">enabled</span><span class="sxs-lookup"><span data-stu-id="087b9-118">enabled</span></span>|<span data-ttu-id="087b9-119">双面</span><span class="sxs-lookup"><span data-stu-id="087b9-119">2</span></span>|<span data-ttu-id="087b9-120">已启用全局设备运行状况脚本并准备好使用</span><span class="sxs-lookup"><span data-stu-id="087b9-120">Global device health scripts are enabled and ready to use</span></span>|



