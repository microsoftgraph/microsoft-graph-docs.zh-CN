---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据, 如 Watson。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c36e2c5467c1a42a9cde44bedd6c8307e77e848d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028369"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="3f0d1-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3f0d1-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="3f0d1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f0d1-105">允许设备发送诊断和使用遥测数据, 如 Watson。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="3f0d1-106">成员</span><span class="sxs-lookup"><span data-stu-id="3f0d1-106">Members</span></span>
|<span data-ttu-id="3f0d1-107">成员</span><span class="sxs-lookup"><span data-stu-id="3f0d1-107">Member</span></span>|<span data-ttu-id="3f0d1-108">值</span><span class="sxs-lookup"><span data-stu-id="3f0d1-108">Value</span></span>|<span data-ttu-id="3f0d1-109">说明</span><span class="sxs-lookup"><span data-stu-id="3f0d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f0d1-110">定制</span><span class="sxs-lookup"><span data-stu-id="3f0d1-110">userDefined</span></span>|<span data-ttu-id="3f0d1-111">0</span><span class="sxs-lookup"><span data-stu-id="3f0d1-111">0</span></span>|<span data-ttu-id="3f0d1-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-112">Allow the user to set.</span></span>|
|<span data-ttu-id="3f0d1-113">无</span><span class="sxs-lookup"><span data-stu-id="3f0d1-113">none</span></span>|<span data-ttu-id="3f0d1-114">1</span><span class="sxs-lookup"><span data-stu-id="3f0d1-114">1</span></span>|<span data-ttu-id="3f0d1-115">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="3f0d1-116">注意: 此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="3f0d1-117">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="3f0d1-118">vba</span><span class="sxs-lookup"><span data-stu-id="3f0d1-118">basic</span></span>|<span data-ttu-id="3f0d1-119">双面</span><span class="sxs-lookup"><span data-stu-id="3f0d1-119">2</span></span>|<span data-ttu-id="3f0d1-120">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="3f0d1-121">有所</span><span class="sxs-lookup"><span data-stu-id="3f0d1-121">enhanced</span></span>|<span data-ttu-id="3f0d1-122">第三章</span><span class="sxs-lookup"><span data-stu-id="3f0d1-122">3</span></span>|<span data-ttu-id="3f0d1-123">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="3f0d1-124">全</span><span class="sxs-lookup"><span data-stu-id="3f0d1-124">full</span></span>|<span data-ttu-id="3f0d1-125">4</span><span class="sxs-lookup"><span data-stu-id="3f0d1-125">4</span></span>|<span data-ttu-id="3f0d1-126">发送包含诊断数据 (如系统状态) 的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="3f0d1-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



