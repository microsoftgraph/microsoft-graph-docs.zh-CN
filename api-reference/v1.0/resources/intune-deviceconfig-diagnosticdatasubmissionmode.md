---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据，如 Watson。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 15abccb0bf2171e62c2b468ecf5c3078e052ea75
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359374"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="0df10-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0df10-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="0df10-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0df10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0df10-105">允许设备发送诊断和使用遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="0df10-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="0df10-106">成员</span><span class="sxs-lookup"><span data-stu-id="0df10-106">Members</span></span>
|<span data-ttu-id="0df10-107">成员</span><span class="sxs-lookup"><span data-stu-id="0df10-107">Member</span></span>|<span data-ttu-id="0df10-108">值</span><span class="sxs-lookup"><span data-stu-id="0df10-108">Value</span></span>|<span data-ttu-id="0df10-109">说明</span><span class="sxs-lookup"><span data-stu-id="0df10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df10-110">定制</span><span class="sxs-lookup"><span data-stu-id="0df10-110">userDefined</span></span>|<span data-ttu-id="0df10-111">0</span><span class="sxs-lookup"><span data-stu-id="0df10-111">0</span></span>|<span data-ttu-id="0df10-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="0df10-112">Allow the user to set.</span></span>|
|<span data-ttu-id="0df10-113">无</span><span class="sxs-lookup"><span data-stu-id="0df10-113">none</span></span>|<span data-ttu-id="0df10-114">1</span><span class="sxs-lookup"><span data-stu-id="0df10-114">1</span></span>|<span data-ttu-id="0df10-115">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="0df10-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="0df10-116">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="0df10-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="0df10-117">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="0df10-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="0df10-118">vba</span><span class="sxs-lookup"><span data-stu-id="0df10-118">basic</span></span>|<span data-ttu-id="0df10-119">双面</span><span class="sxs-lookup"><span data-stu-id="0df10-119">2</span></span>|<span data-ttu-id="0df10-120">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="0df10-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="0df10-121">有所</span><span class="sxs-lookup"><span data-stu-id="0df10-121">enhanced</span></span>|<span data-ttu-id="0df10-122">第三章</span><span class="sxs-lookup"><span data-stu-id="0df10-122">3</span></span>|<span data-ttu-id="0df10-123">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="0df10-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="0df10-124">全</span><span class="sxs-lookup"><span data-stu-id="0df10-124">full</span></span>|<span data-ttu-id="0df10-125">4</span><span class="sxs-lookup"><span data-stu-id="0df10-125">4</span></span>|<span data-ttu-id="0df10-126">发送包含诊断数据（如系统状态）的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="0df10-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




