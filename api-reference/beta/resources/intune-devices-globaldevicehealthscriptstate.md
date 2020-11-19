---
title: globalDeviceHealthScriptState 枚举类型
description: 指示是否启用全局设备运行状况脚本并将其状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7883fe642b4e7772caa6a13241db0b8e62d7fb98
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299092"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="49c5c-103">globalDeviceHealthScriptState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49c5c-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="49c5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49c5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49c5c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49c5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49c5c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49c5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49c5c-107">指示是否启用全局设备运行状况脚本并将其状态</span><span class="sxs-lookup"><span data-stu-id="49c5c-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="49c5c-108">成员</span><span class="sxs-lookup"><span data-stu-id="49c5c-108">Members</span></span>
|<span data-ttu-id="49c5c-109">成员</span><span class="sxs-lookup"><span data-stu-id="49c5c-109">Member</span></span>|<span data-ttu-id="49c5c-110">值</span><span class="sxs-lookup"><span data-stu-id="49c5c-110">Value</span></span>|<span data-ttu-id="49c5c-111">Description</span><span class="sxs-lookup"><span data-stu-id="49c5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49c5c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="49c5c-112">notConfigured</span></span>|<span data-ttu-id="49c5c-113">0</span><span class="sxs-lookup"><span data-stu-id="49c5c-113">0</span></span>|<span data-ttu-id="49c5c-114">未配置全局设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="49c5c-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="49c5c-115">决</span><span class="sxs-lookup"><span data-stu-id="49c5c-115">pending</span></span>|<span data-ttu-id="49c5c-116">1</span><span class="sxs-lookup"><span data-stu-id="49c5c-116">1</span></span>|<span data-ttu-id="49c5c-117">已配置全局设备运行状况脚本，但未完全启用</span><span class="sxs-lookup"><span data-stu-id="49c5c-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="49c5c-118">enabled</span><span class="sxs-lookup"><span data-stu-id="49c5c-118">enabled</span></span>|<span data-ttu-id="49c5c-119">双面</span><span class="sxs-lookup"><span data-stu-id="49c5c-119">2</span></span>|<span data-ttu-id="49c5c-120">已启用全局设备运行状况脚本并准备好使用</span><span class="sxs-lookup"><span data-stu-id="49c5c-120">Global device health scripts are enabled and ready to use</span></span>|




