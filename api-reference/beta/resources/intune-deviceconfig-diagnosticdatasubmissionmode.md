---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据, 如 Watson。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ea3267ca6c692ce916a1b8e063ac937c38618e2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802196"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="f0965-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f0965-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="f0965-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0965-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0965-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0965-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0965-106">允许设备发送诊断和使用遥测数据, 如 Watson。</span><span class="sxs-lookup"><span data-stu-id="f0965-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="f0965-107">成员</span><span class="sxs-lookup"><span data-stu-id="f0965-107">Members</span></span>
|<span data-ttu-id="f0965-108">成员</span><span class="sxs-lookup"><span data-stu-id="f0965-108">Member</span></span>|<span data-ttu-id="f0965-109">值</span><span class="sxs-lookup"><span data-stu-id="f0965-109">Value</span></span>|<span data-ttu-id="f0965-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0965-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0965-111">定制</span><span class="sxs-lookup"><span data-stu-id="f0965-111">userDefined</span></span>|<span data-ttu-id="f0965-112">0</span><span class="sxs-lookup"><span data-stu-id="f0965-112">0</span></span>|<span data-ttu-id="f0965-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="f0965-113">Allow the user to set.</span></span>|
|<span data-ttu-id="f0965-114">无</span><span class="sxs-lookup"><span data-stu-id="f0965-114">none</span></span>|<span data-ttu-id="f0965-115">1</span><span class="sxs-lookup"><span data-stu-id="f0965-115">1</span></span>|<span data-ttu-id="f0965-116">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="f0965-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="f0965-117">注意: 此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="f0965-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="f0965-118">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="f0965-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="f0965-119">vba</span><span class="sxs-lookup"><span data-stu-id="f0965-119">basic</span></span>|<span data-ttu-id="f0965-120">双面</span><span class="sxs-lookup"><span data-stu-id="f0965-120">2</span></span>|<span data-ttu-id="f0965-121">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="f0965-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="f0965-122">有所</span><span class="sxs-lookup"><span data-stu-id="f0965-122">enhanced</span></span>|<span data-ttu-id="f0965-123">第三章</span><span class="sxs-lookup"><span data-stu-id="f0965-123">3</span></span>|<span data-ttu-id="f0965-124">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="f0965-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="f0965-125">全</span><span class="sxs-lookup"><span data-stu-id="f0965-125">full</span></span>|<span data-ttu-id="f0965-126">4</span><span class="sxs-lookup"><span data-stu-id="f0965-126">4</span></span>|<span data-ttu-id="f0965-127">发送包含诊断数据 (如系统状态) 的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="f0965-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





