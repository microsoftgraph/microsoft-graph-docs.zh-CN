---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用情况遥测数据，例如 Watson。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 172ac80e4491d238414777c4d1d30d9f969f2a39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755082"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="8d897-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8d897-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="8d897-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d897-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d897-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d897-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d897-106">允许设备发送诊断和使用情况遥测数据，例如 Watson。</span><span class="sxs-lookup"><span data-stu-id="8d897-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="8d897-107">成员</span><span class="sxs-lookup"><span data-stu-id="8d897-107">Members</span></span>
|<span data-ttu-id="8d897-108">成员</span><span class="sxs-lookup"><span data-stu-id="8d897-108">Member</span></span>|<span data-ttu-id="8d897-109">值</span><span class="sxs-lookup"><span data-stu-id="8d897-109">Value</span></span>|<span data-ttu-id="8d897-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d897-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d897-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="8d897-111">userDefined</span></span>|<span data-ttu-id="8d897-112">0</span><span class="sxs-lookup"><span data-stu-id="8d897-112">0</span></span>|<span data-ttu-id="8d897-113">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="8d897-113">Allow the user to set.</span></span>|
|<span data-ttu-id="8d897-114">无</span><span class="sxs-lookup"><span data-stu-id="8d897-114">none</span></span>|<span data-ttu-id="8d897-115">1</span><span class="sxs-lookup"><span data-stu-id="8d897-115">1</span></span>|<span data-ttu-id="8d897-116">不会从操作系统组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="8d897-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="8d897-117">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="8d897-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="8d897-118">在其他设备上使用此设置等效于将值设置为 1。</span><span class="sxs-lookup"><span data-stu-id="8d897-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="8d897-119">basic</span><span class="sxs-lookup"><span data-stu-id="8d897-119">basic</span></span>|<span data-ttu-id="8d897-120">2</span><span class="sxs-lookup"><span data-stu-id="8d897-120">2</span></span>|<span data-ttu-id="8d897-121">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="8d897-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="8d897-122">增强</span><span class="sxs-lookup"><span data-stu-id="8d897-122">enhanced</span></span>|<span data-ttu-id="8d897-123">3</span><span class="sxs-lookup"><span data-stu-id="8d897-123">3</span></span>|<span data-ttu-id="8d897-124">发送增强的遥测数据，包括使用情况和见解数据。</span><span class="sxs-lookup"><span data-stu-id="8d897-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="8d897-125">full</span><span class="sxs-lookup"><span data-stu-id="8d897-125">full</span></span>|<span data-ttu-id="8d897-126">4 </span><span class="sxs-lookup"><span data-stu-id="8d897-126">4</span></span>|<span data-ttu-id="8d897-127">发送完整的遥测数据，包括诊断数据，如系统状态。</span><span class="sxs-lookup"><span data-stu-id="8d897-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




