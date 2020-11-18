---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据，如 Watson。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7c6198d3fb0bc7b714658561e1f4036153bd36fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199355"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="851c6-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="851c6-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="851c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="851c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="851c6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="851c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="851c6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="851c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="851c6-107">允许设备发送诊断和使用遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="851c6-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="851c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="851c6-108">Members</span></span>
|<span data-ttu-id="851c6-109">成员</span><span class="sxs-lookup"><span data-stu-id="851c6-109">Member</span></span>|<span data-ttu-id="851c6-110">值</span><span class="sxs-lookup"><span data-stu-id="851c6-110">Value</span></span>|<span data-ttu-id="851c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="851c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="851c6-112">定制</span><span class="sxs-lookup"><span data-stu-id="851c6-112">userDefined</span></span>|<span data-ttu-id="851c6-113">0</span><span class="sxs-lookup"><span data-stu-id="851c6-113">0</span></span>|<span data-ttu-id="851c6-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="851c6-114">Allow the user to set.</span></span>|
|<span data-ttu-id="851c6-115">无</span><span class="sxs-lookup"><span data-stu-id="851c6-115">none</span></span>|<span data-ttu-id="851c6-116">1</span><span class="sxs-lookup"><span data-stu-id="851c6-116">1</span></span>|<span data-ttu-id="851c6-117">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="851c6-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="851c6-118">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="851c6-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="851c6-119">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="851c6-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="851c6-120">vba</span><span class="sxs-lookup"><span data-stu-id="851c6-120">basic</span></span>|<span data-ttu-id="851c6-121">双面</span><span class="sxs-lookup"><span data-stu-id="851c6-121">2</span></span>|<span data-ttu-id="851c6-122">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="851c6-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="851c6-123">有所</span><span class="sxs-lookup"><span data-stu-id="851c6-123">enhanced</span></span>|<span data-ttu-id="851c6-124">第三章</span><span class="sxs-lookup"><span data-stu-id="851c6-124">3</span></span>|<span data-ttu-id="851c6-125">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="851c6-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="851c6-126">全</span><span class="sxs-lookup"><span data-stu-id="851c6-126">full</span></span>|<span data-ttu-id="851c6-127">4 </span><span class="sxs-lookup"><span data-stu-id="851c6-127">4</span></span>|<span data-ttu-id="851c6-128">发送包含诊断数据（如系统状态）的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="851c6-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




