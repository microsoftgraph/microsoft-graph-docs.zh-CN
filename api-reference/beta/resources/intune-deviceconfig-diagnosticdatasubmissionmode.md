---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许该设备发送诊断和使用情况的遥测数据，如 Watson。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422255"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="6f40e-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6f40e-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="6f40e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6f40e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f40e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f40e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f40e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f40e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f40e-107">允许该设备发送诊断和使用情况的遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="6f40e-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="6f40e-108">成员</span><span class="sxs-lookup"><span data-stu-id="6f40e-108">Members</span></span>
|<span data-ttu-id="6f40e-109">成员</span><span class="sxs-lookup"><span data-stu-id="6f40e-109">Member</span></span>|<span data-ttu-id="6f40e-110">值</span><span class="sxs-lookup"><span data-stu-id="6f40e-110">Value</span></span>|<span data-ttu-id="6f40e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f40e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f40e-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="6f40e-112">userDefined</span></span>|<span data-ttu-id="6f40e-113">0</span><span class="sxs-lookup"><span data-stu-id="6f40e-113">0</span></span>|<span data-ttu-id="6f40e-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="6f40e-114">Allow the user to set.</span></span>|
|<span data-ttu-id="6f40e-115">无</span><span class="sxs-lookup"><span data-stu-id="6f40e-115">none</span></span>|<span data-ttu-id="6f40e-116">1</span><span class="sxs-lookup"><span data-stu-id="6f40e-116">1</span></span>|<span data-ttu-id="6f40e-117">从操作系统组件不发送任何遥测数据。</span><span class="sxs-lookup"><span data-stu-id="6f40e-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="6f40e-118">注意： 此值才适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="6f40e-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="6f40e-119">在其他设备上使用此设置等同于设置 1 的值。</span><span class="sxs-lookup"><span data-stu-id="6f40e-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="6f40e-120">基本</span><span class="sxs-lookup"><span data-stu-id="6f40e-120">basic</span></span>|<span data-ttu-id="6f40e-121">2</span><span class="sxs-lookup"><span data-stu-id="6f40e-121">2</span></span>|<span data-ttu-id="6f40e-122">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="6f40e-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="6f40e-123">增强</span><span class="sxs-lookup"><span data-stu-id="6f40e-123">enhanced</span></span>|<span data-ttu-id="6f40e-124">3</span><span class="sxs-lookup"><span data-stu-id="6f40e-124">3</span></span>|<span data-ttu-id="6f40e-125">发送增强，包括使用情况和见解数据的遥测数据。</span><span class="sxs-lookup"><span data-stu-id="6f40e-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="6f40e-126">完整</span><span class="sxs-lookup"><span data-stu-id="6f40e-126">full</span></span>|<span data-ttu-id="6f40e-127">4</span><span class="sxs-lookup"><span data-stu-id="6f40e-127">4</span></span>|<span data-ttu-id="6f40e-128">发送完全遥测数据，包括诊断数据，如系统状态。</span><span class="sxs-lookup"><span data-stu-id="6f40e-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




