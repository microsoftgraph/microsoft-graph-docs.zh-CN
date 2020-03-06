---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据，如 Watson。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 838f90e8396be1ae3a55ea28f749cfd5b42edd01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532552"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="a01c4-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a01c4-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="a01c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a01c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a01c4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a01c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a01c4-106">允许设备发送诊断和使用遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="a01c4-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="a01c4-107">成员</span><span class="sxs-lookup"><span data-stu-id="a01c4-107">Members</span></span>
|<span data-ttu-id="a01c4-108">成员</span><span class="sxs-lookup"><span data-stu-id="a01c4-108">Member</span></span>|<span data-ttu-id="a01c4-109">值</span><span class="sxs-lookup"><span data-stu-id="a01c4-109">Value</span></span>|<span data-ttu-id="a01c4-110">说明</span><span class="sxs-lookup"><span data-stu-id="a01c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a01c4-111">定制</span><span class="sxs-lookup"><span data-stu-id="a01c4-111">userDefined</span></span>|<span data-ttu-id="a01c4-112">0</span><span class="sxs-lookup"><span data-stu-id="a01c4-112">0</span></span>|<span data-ttu-id="a01c4-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="a01c4-113">Allow the user to set.</span></span>|
|<span data-ttu-id="a01c4-114">无</span><span class="sxs-lookup"><span data-stu-id="a01c4-114">none</span></span>|<span data-ttu-id="a01c4-115">1 </span><span class="sxs-lookup"><span data-stu-id="a01c4-115">1</span></span>|<span data-ttu-id="a01c4-116">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="a01c4-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="a01c4-117">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="a01c4-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="a01c4-118">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="a01c4-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="a01c4-119">vba</span><span class="sxs-lookup"><span data-stu-id="a01c4-119">basic</span></span>|<span data-ttu-id="a01c4-120">2 </span><span class="sxs-lookup"><span data-stu-id="a01c4-120">2</span></span>|<span data-ttu-id="a01c4-121">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="a01c4-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="a01c4-122">有所</span><span class="sxs-lookup"><span data-stu-id="a01c4-122">enhanced</span></span>|<span data-ttu-id="a01c4-123">3 </span><span class="sxs-lookup"><span data-stu-id="a01c4-123">3</span></span>|<span data-ttu-id="a01c4-124">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="a01c4-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="a01c4-125">全</span><span class="sxs-lookup"><span data-stu-id="a01c4-125">full</span></span>|<span data-ttu-id="a01c4-126">4 </span><span class="sxs-lookup"><span data-stu-id="a01c4-126">4</span></span>|<span data-ttu-id="a01c4-127">发送包含诊断数据（如系统状态）的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="a01c4-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




