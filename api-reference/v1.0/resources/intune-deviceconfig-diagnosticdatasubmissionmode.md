---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许该设备发送诊断和使用情况的遥测数据，如 Watson。
localization_priority: Normal
ms.openlocfilehash: 1654e9c5c94fd79bbda0d77ef84101fb9fb92d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812780"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="9b48a-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b48a-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="9b48a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9b48a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b48a-105">允许该设备发送诊断和使用情况的遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="9b48a-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="9b48a-106">成员</span><span class="sxs-lookup"><span data-stu-id="9b48a-106">Members</span></span>
|<span data-ttu-id="9b48a-107">成员</span><span class="sxs-lookup"><span data-stu-id="9b48a-107">Member</span></span>|<span data-ttu-id="9b48a-108">值</span><span class="sxs-lookup"><span data-stu-id="9b48a-108">Value</span></span>|<span data-ttu-id="9b48a-109">Description</span><span class="sxs-lookup"><span data-stu-id="9b48a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b48a-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="9b48a-110">userDefined</span></span>|<span data-ttu-id="9b48a-111">0</span><span class="sxs-lookup"><span data-stu-id="9b48a-111">0</span></span>|<span data-ttu-id="9b48a-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="9b48a-112">Allow the user to set.</span></span>|
|<span data-ttu-id="9b48a-113">无</span><span class="sxs-lookup"><span data-stu-id="9b48a-113">none</span></span>|<span data-ttu-id="9b48a-114">1</span><span class="sxs-lookup"><span data-stu-id="9b48a-114">1</span></span>|<span data-ttu-id="9b48a-115">从操作系统组件不发送任何遥测数据。</span><span class="sxs-lookup"><span data-stu-id="9b48a-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="9b48a-116">注意： 此值才适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="9b48a-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="9b48a-117">在其他设备上使用此设置等同于设置 1 的值。</span><span class="sxs-lookup"><span data-stu-id="9b48a-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="9b48a-118">基本</span><span class="sxs-lookup"><span data-stu-id="9b48a-118">basic</span></span>|<span data-ttu-id="9b48a-119">2</span><span class="sxs-lookup"><span data-stu-id="9b48a-119">2</span></span>|<span data-ttu-id="9b48a-120">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="9b48a-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="9b48a-121">增强</span><span class="sxs-lookup"><span data-stu-id="9b48a-121">enhanced</span></span>|<span data-ttu-id="9b48a-122">3</span><span class="sxs-lookup"><span data-stu-id="9b48a-122">3</span></span>|<span data-ttu-id="9b48a-123">发送增强，包括使用情况和见解数据的遥测数据。</span><span class="sxs-lookup"><span data-stu-id="9b48a-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="9b48a-124">完整</span><span class="sxs-lookup"><span data-stu-id="9b48a-124">full</span></span>|<span data-ttu-id="9b48a-125">4</span><span class="sxs-lookup"><span data-stu-id="9b48a-125">4</span></span>|<span data-ttu-id="9b48a-126">发送完全遥测数据，包括诊断数据，如系统状态。</span><span class="sxs-lookup"><span data-stu-id="9b48a-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



