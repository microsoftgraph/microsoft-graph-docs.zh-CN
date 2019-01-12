---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许该设备发送诊断和使用情况的遥测数据，如 Watson。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912944"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="03f52-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="03f52-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="03f52-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="03f52-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03f52-105">允许该设备发送诊断和使用情况的遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="03f52-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="03f52-106">成员</span><span class="sxs-lookup"><span data-stu-id="03f52-106">Members</span></span>
|<span data-ttu-id="03f52-107">成员</span><span class="sxs-lookup"><span data-stu-id="03f52-107">Member</span></span>|<span data-ttu-id="03f52-108">值</span><span class="sxs-lookup"><span data-stu-id="03f52-108">Value</span></span>|<span data-ttu-id="03f52-109">说明</span><span class="sxs-lookup"><span data-stu-id="03f52-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f52-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="03f52-110">userDefined</span></span>|<span data-ttu-id="03f52-111">0</span><span class="sxs-lookup"><span data-stu-id="03f52-111">0</span></span>|<span data-ttu-id="03f52-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="03f52-112">Allow the user to set.</span></span>|
|<span data-ttu-id="03f52-113">无</span><span class="sxs-lookup"><span data-stu-id="03f52-113">none</span></span>|<span data-ttu-id="03f52-114">1</span><span class="sxs-lookup"><span data-stu-id="03f52-114">1</span></span>|<span data-ttu-id="03f52-115">从操作系统组件不发送任何遥测数据。</span><span class="sxs-lookup"><span data-stu-id="03f52-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="03f52-116">注意： 此值才适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="03f52-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="03f52-117">在其他设备上使用此设置等同于设置 1 的值。</span><span class="sxs-lookup"><span data-stu-id="03f52-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="03f52-118">基本</span><span class="sxs-lookup"><span data-stu-id="03f52-118">basic</span></span>|<span data-ttu-id="03f52-119">2</span><span class="sxs-lookup"><span data-stu-id="03f52-119">2</span></span>|<span data-ttu-id="03f52-120">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="03f52-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="03f52-121">增强</span><span class="sxs-lookup"><span data-stu-id="03f52-121">enhanced</span></span>|<span data-ttu-id="03f52-122">3</span><span class="sxs-lookup"><span data-stu-id="03f52-122">3</span></span>|<span data-ttu-id="03f52-123">发送增强，包括使用情况和见解数据的遥测数据。</span><span class="sxs-lookup"><span data-stu-id="03f52-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="03f52-124">完整</span><span class="sxs-lookup"><span data-stu-id="03f52-124">full</span></span>|<span data-ttu-id="03f52-125">4</span><span class="sxs-lookup"><span data-stu-id="03f52-125">4</span></span>|<span data-ttu-id="03f52-126">发送完全遥测数据，包括诊断数据，如系统状态。</span><span class="sxs-lookup"><span data-stu-id="03f52-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



