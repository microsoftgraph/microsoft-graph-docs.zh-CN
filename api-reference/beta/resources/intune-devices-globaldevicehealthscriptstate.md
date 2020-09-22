---
title: globalDeviceHealthScriptState 枚举类型
description: 指示是否启用全局设备运行状况脚本并将其状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c2e9ed441cbc28c0f3a7a3184bd584cbc34fb957
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081396"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="5c846-103">globalDeviceHealthScriptState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5c846-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="5c846-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c846-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c846-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c846-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c846-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c846-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c846-107">指示是否启用全局设备运行状况脚本并将其状态</span><span class="sxs-lookup"><span data-stu-id="5c846-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="5c846-108">成员</span><span class="sxs-lookup"><span data-stu-id="5c846-108">Members</span></span>
|<span data-ttu-id="5c846-109">成员</span><span class="sxs-lookup"><span data-stu-id="5c846-109">Member</span></span>|<span data-ttu-id="5c846-110">值</span><span class="sxs-lookup"><span data-stu-id="5c846-110">Value</span></span>|<span data-ttu-id="5c846-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c846-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c846-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5c846-112">notConfigured</span></span>|<span data-ttu-id="5c846-113">0</span><span class="sxs-lookup"><span data-stu-id="5c846-113">0</span></span>|<span data-ttu-id="5c846-114">未配置全局设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="5c846-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="5c846-115">决</span><span class="sxs-lookup"><span data-stu-id="5c846-115">pending</span></span>|<span data-ttu-id="5c846-116">1 </span><span class="sxs-lookup"><span data-stu-id="5c846-116">1</span></span>|<span data-ttu-id="5c846-117">已配置全局设备运行状况脚本，但未完全启用</span><span class="sxs-lookup"><span data-stu-id="5c846-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="5c846-118">enabled</span><span class="sxs-lookup"><span data-stu-id="5c846-118">enabled</span></span>|<span data-ttu-id="5c846-119">2 </span><span class="sxs-lookup"><span data-stu-id="5c846-119">2</span></span>|<span data-ttu-id="5c846-120">已启用全局设备运行状况脚本并准备好使用</span><span class="sxs-lookup"><span data-stu-id="5c846-120">Global device health scripts are enabled and ready to use</span></span>|






