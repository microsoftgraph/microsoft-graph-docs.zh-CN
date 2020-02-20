---
title: globalDeviceHealthScriptState 枚举类型
description: 指示是否启用全局设备运行状况脚本并将其状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3f154e760398116ca6c22d21d6947c08a10e0eb4
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163820"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="05424-103">globalDeviceHealthScriptState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="05424-103">globalDeviceHealthScriptState enum type</span></span>

> <span data-ttu-id="05424-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05424-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05424-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05424-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05424-106">指示是否启用全局设备运行状况脚本并将其状态</span><span class="sxs-lookup"><span data-stu-id="05424-106">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="05424-107">成员</span><span class="sxs-lookup"><span data-stu-id="05424-107">Members</span></span>
|<span data-ttu-id="05424-108">成员</span><span class="sxs-lookup"><span data-stu-id="05424-108">Member</span></span>|<span data-ttu-id="05424-109">值</span><span class="sxs-lookup"><span data-stu-id="05424-109">Value</span></span>|<span data-ttu-id="05424-110">说明</span><span class="sxs-lookup"><span data-stu-id="05424-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05424-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="05424-111">notConfigured</span></span>|<span data-ttu-id="05424-112">0</span><span class="sxs-lookup"><span data-stu-id="05424-112">0</span></span>|<span data-ttu-id="05424-113">未配置全局设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="05424-113">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="05424-114">决</span><span class="sxs-lookup"><span data-stu-id="05424-114">pending</span></span>|<span data-ttu-id="05424-115">1</span><span class="sxs-lookup"><span data-stu-id="05424-115">1</span></span>|<span data-ttu-id="05424-116">已配置全局设备运行状况脚本，但未完全启用</span><span class="sxs-lookup"><span data-stu-id="05424-116">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="05424-117">enabled</span><span class="sxs-lookup"><span data-stu-id="05424-117">enabled</span></span>|<span data-ttu-id="05424-118">双面</span><span class="sxs-lookup"><span data-stu-id="05424-118">2</span></span>|<span data-ttu-id="05424-119">已启用全局设备运行状况脚本并准备好使用</span><span class="sxs-lookup"><span data-stu-id="05424-119">Global device health scripts are enabled and ready to use</span></span>|



