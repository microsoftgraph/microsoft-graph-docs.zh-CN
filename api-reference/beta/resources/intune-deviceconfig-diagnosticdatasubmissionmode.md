---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据, 如 Watson。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fce6bbe40d985c15c5455c3b83de88ced4cce768
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332685"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="1c082-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1c082-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="1c082-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c082-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c082-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c082-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c082-106">允许设备发送诊断和使用遥测数据, 如 Watson。</span><span class="sxs-lookup"><span data-stu-id="1c082-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="1c082-107">成员</span><span class="sxs-lookup"><span data-stu-id="1c082-107">Members</span></span>
|<span data-ttu-id="1c082-108">成员</span><span class="sxs-lookup"><span data-stu-id="1c082-108">Member</span></span>|<span data-ttu-id="1c082-109">值</span><span class="sxs-lookup"><span data-stu-id="1c082-109">Value</span></span>|<span data-ttu-id="1c082-110">说明</span><span class="sxs-lookup"><span data-stu-id="1c082-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c082-111">定制</span><span class="sxs-lookup"><span data-stu-id="1c082-111">userDefined</span></span>|<span data-ttu-id="1c082-112">0</span><span class="sxs-lookup"><span data-stu-id="1c082-112">0</span></span>|<span data-ttu-id="1c082-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="1c082-113">Allow the user to set.</span></span>|
|<span data-ttu-id="1c082-114">无</span><span class="sxs-lookup"><span data-stu-id="1c082-114">none</span></span>|<span data-ttu-id="1c082-115">1</span><span class="sxs-lookup"><span data-stu-id="1c082-115">1</span></span>|<span data-ttu-id="1c082-116">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="1c082-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="1c082-117">注意: 此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="1c082-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="1c082-118">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="1c082-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="1c082-119">vba</span><span class="sxs-lookup"><span data-stu-id="1c082-119">basic</span></span>|<span data-ttu-id="1c082-120">双面</span><span class="sxs-lookup"><span data-stu-id="1c082-120">2</span></span>|<span data-ttu-id="1c082-121">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="1c082-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="1c082-122">有所</span><span class="sxs-lookup"><span data-stu-id="1c082-122">enhanced</span></span>|<span data-ttu-id="1c082-123">第三章</span><span class="sxs-lookup"><span data-stu-id="1c082-123">3</span></span>|<span data-ttu-id="1c082-124">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="1c082-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="1c082-125">全</span><span class="sxs-lookup"><span data-stu-id="1c082-125">full</span></span>|<span data-ttu-id="1c082-126">4</span><span class="sxs-lookup"><span data-stu-id="1c082-126">4</span></span>|<span data-ttu-id="1c082-127">发送包含诊断数据 (如系统状态) 的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="1c082-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



