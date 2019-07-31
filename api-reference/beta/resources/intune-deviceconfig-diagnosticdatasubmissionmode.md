---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据, 如 Watson。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 788da8fd9a239bf26dfd2d9e8d8fbf308d059784
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004538"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="d1ef5-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d1ef5-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="d1ef5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1ef5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1ef5-106">允许设备发送诊断和使用遥测数据, 如 Watson。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="d1ef5-107">成员</span><span class="sxs-lookup"><span data-stu-id="d1ef5-107">Members</span></span>
|<span data-ttu-id="d1ef5-108">成员</span><span class="sxs-lookup"><span data-stu-id="d1ef5-108">Member</span></span>|<span data-ttu-id="d1ef5-109">值</span><span class="sxs-lookup"><span data-stu-id="d1ef5-109">Value</span></span>|<span data-ttu-id="d1ef5-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1ef5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1ef5-111">定制</span><span class="sxs-lookup"><span data-stu-id="d1ef5-111">userDefined</span></span>|<span data-ttu-id="d1ef5-112">0</span><span class="sxs-lookup"><span data-stu-id="d1ef5-112">0</span></span>|<span data-ttu-id="d1ef5-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-113">Allow the user to set.</span></span>|
|<span data-ttu-id="d1ef5-114">无</span><span class="sxs-lookup"><span data-stu-id="d1ef5-114">none</span></span>|<span data-ttu-id="d1ef5-115">1</span><span class="sxs-lookup"><span data-stu-id="d1ef5-115">1</span></span>|<span data-ttu-id="d1ef5-116">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="d1ef5-117">注意: 此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="d1ef5-118">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="d1ef5-119">vba</span><span class="sxs-lookup"><span data-stu-id="d1ef5-119">basic</span></span>|<span data-ttu-id="d1ef5-120">双面</span><span class="sxs-lookup"><span data-stu-id="d1ef5-120">2</span></span>|<span data-ttu-id="d1ef5-121">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="d1ef5-122">有所</span><span class="sxs-lookup"><span data-stu-id="d1ef5-122">enhanced</span></span>|<span data-ttu-id="d1ef5-123">第三章</span><span class="sxs-lookup"><span data-stu-id="d1ef5-123">3</span></span>|<span data-ttu-id="d1ef5-124">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="d1ef5-125">全</span><span class="sxs-lookup"><span data-stu-id="d1ef5-125">full</span></span>|<span data-ttu-id="d1ef5-126">4</span><span class="sxs-lookup"><span data-stu-id="d1ef5-126">4</span></span>|<span data-ttu-id="d1ef5-127">发送包含诊断数据 (如系统状态) 的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="d1ef5-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





