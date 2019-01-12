---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许该设备发送诊断和使用情况的遥测数据，如 Watson。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: d1ba4d2cd9be740b23502ec4c0154caa2be07f3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948527"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="17e49-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="17e49-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="17e49-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="17e49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17e49-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17e49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17e49-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="17e49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17e49-107">允许该设备发送诊断和使用情况的遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="17e49-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="17e49-108">成员</span><span class="sxs-lookup"><span data-stu-id="17e49-108">Members</span></span>
|<span data-ttu-id="17e49-109">成员</span><span class="sxs-lookup"><span data-stu-id="17e49-109">Member</span></span>|<span data-ttu-id="17e49-110">值</span><span class="sxs-lookup"><span data-stu-id="17e49-110">Value</span></span>|<span data-ttu-id="17e49-111">Description</span><span class="sxs-lookup"><span data-stu-id="17e49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17e49-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="17e49-112">userDefined</span></span>|<span data-ttu-id="17e49-113">0</span><span class="sxs-lookup"><span data-stu-id="17e49-113">0</span></span>|<span data-ttu-id="17e49-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="17e49-114">Allow the user to set.</span></span>|
|<span data-ttu-id="17e49-115">无</span><span class="sxs-lookup"><span data-stu-id="17e49-115">none</span></span>|<span data-ttu-id="17e49-116">1</span><span class="sxs-lookup"><span data-stu-id="17e49-116">1</span></span>|<span data-ttu-id="17e49-117">从操作系统组件不发送任何遥测数据。</span><span class="sxs-lookup"><span data-stu-id="17e49-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="17e49-118">注意： 此值才适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="17e49-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="17e49-119">在其他设备上使用此设置等同于设置 1 的值。</span><span class="sxs-lookup"><span data-stu-id="17e49-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="17e49-120">基本</span><span class="sxs-lookup"><span data-stu-id="17e49-120">basic</span></span>|<span data-ttu-id="17e49-121">2</span><span class="sxs-lookup"><span data-stu-id="17e49-121">2</span></span>|<span data-ttu-id="17e49-122">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="17e49-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="17e49-123">增强</span><span class="sxs-lookup"><span data-stu-id="17e49-123">enhanced</span></span>|<span data-ttu-id="17e49-124">3</span><span class="sxs-lookup"><span data-stu-id="17e49-124">3</span></span>|<span data-ttu-id="17e49-125">发送增强，包括使用情况和见解数据的遥测数据。</span><span class="sxs-lookup"><span data-stu-id="17e49-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="17e49-126">完整</span><span class="sxs-lookup"><span data-stu-id="17e49-126">full</span></span>|<span data-ttu-id="17e49-127">4</span><span class="sxs-lookup"><span data-stu-id="17e49-127">4</span></span>|<span data-ttu-id="17e49-128">发送完全遥测数据，包括诊断数据，如系统状态。</span><span class="sxs-lookup"><span data-stu-id="17e49-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





