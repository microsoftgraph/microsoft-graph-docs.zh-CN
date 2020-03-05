---
title: globalDeviceHealthScriptState 枚举类型
description: 指示是否启用全局设备运行状况脚本并将其状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dbdcda672147c1e555727b9f5024744e287a6a6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528575"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="dd43a-103">globalDeviceHealthScriptState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dd43a-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="dd43a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dd43a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd43a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd43a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd43a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd43a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd43a-107">指示是否启用全局设备运行状况脚本并将其状态</span><span class="sxs-lookup"><span data-stu-id="dd43a-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="dd43a-108">成员</span><span class="sxs-lookup"><span data-stu-id="dd43a-108">Members</span></span>
|<span data-ttu-id="dd43a-109">成员</span><span class="sxs-lookup"><span data-stu-id="dd43a-109">Member</span></span>|<span data-ttu-id="dd43a-110">值</span><span class="sxs-lookup"><span data-stu-id="dd43a-110">Value</span></span>|<span data-ttu-id="dd43a-111">说明</span><span class="sxs-lookup"><span data-stu-id="dd43a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd43a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="dd43a-112">notConfigured</span></span>|<span data-ttu-id="dd43a-113">0</span><span class="sxs-lookup"><span data-stu-id="dd43a-113">0</span></span>|<span data-ttu-id="dd43a-114">未配置全局设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="dd43a-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="dd43a-115">决</span><span class="sxs-lookup"><span data-stu-id="dd43a-115">pending</span></span>|<span data-ttu-id="dd43a-116">1 </span><span class="sxs-lookup"><span data-stu-id="dd43a-116">1</span></span>|<span data-ttu-id="dd43a-117">已配置全局设备运行状况脚本，但未完全启用</span><span class="sxs-lookup"><span data-stu-id="dd43a-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="dd43a-118">enabled</span><span class="sxs-lookup"><span data-stu-id="dd43a-118">enabled</span></span>|<span data-ttu-id="dd43a-119">2 </span><span class="sxs-lookup"><span data-stu-id="dd43a-119">2</span></span>|<span data-ttu-id="dd43a-120">已启用全局设备运行状况脚本并准备好使用</span><span class="sxs-lookup"><span data-stu-id="dd43a-120">Global device health scripts are enabled and ready to use</span></span>|



