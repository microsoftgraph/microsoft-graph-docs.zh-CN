---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据，如 Watson。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 80a936c103caa4655addd25f8a21d75d9bc67040
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465686"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="63e58-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63e58-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="63e58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63e58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63e58-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e58-106">允许设备发送诊断和使用遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="63e58-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="63e58-107">成员</span><span class="sxs-lookup"><span data-stu-id="63e58-107">Members</span></span>
|<span data-ttu-id="63e58-108">成员</span><span class="sxs-lookup"><span data-stu-id="63e58-108">Member</span></span>|<span data-ttu-id="63e58-109">值</span><span class="sxs-lookup"><span data-stu-id="63e58-109">Value</span></span>|<span data-ttu-id="63e58-110">说明</span><span class="sxs-lookup"><span data-stu-id="63e58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e58-111">定制</span><span class="sxs-lookup"><span data-stu-id="63e58-111">userDefined</span></span>|<span data-ttu-id="63e58-112">0</span><span class="sxs-lookup"><span data-stu-id="63e58-112">0</span></span>|<span data-ttu-id="63e58-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="63e58-113">Allow the user to set.</span></span>|
|<span data-ttu-id="63e58-114">无</span><span class="sxs-lookup"><span data-stu-id="63e58-114">none</span></span>|<span data-ttu-id="63e58-115">1</span><span class="sxs-lookup"><span data-stu-id="63e58-115">1</span></span>|<span data-ttu-id="63e58-116">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="63e58-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="63e58-117">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="63e58-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="63e58-118">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="63e58-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="63e58-119">vba</span><span class="sxs-lookup"><span data-stu-id="63e58-119">basic</span></span>|<span data-ttu-id="63e58-120">双面</span><span class="sxs-lookup"><span data-stu-id="63e58-120">2</span></span>|<span data-ttu-id="63e58-121">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="63e58-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="63e58-122">有所</span><span class="sxs-lookup"><span data-stu-id="63e58-122">enhanced</span></span>|<span data-ttu-id="63e58-123">第三章</span><span class="sxs-lookup"><span data-stu-id="63e58-123">3</span></span>|<span data-ttu-id="63e58-124">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="63e58-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="63e58-125">全</span><span class="sxs-lookup"><span data-stu-id="63e58-125">full</span></span>|<span data-ttu-id="63e58-126">4 </span><span class="sxs-lookup"><span data-stu-id="63e58-126">4</span></span>|<span data-ttu-id="63e58-127">发送包含诊断数据（如系统状态）的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="63e58-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|







