---
title: diagnosticDataSubmissionMode 枚举类型
description: 允许设备发送诊断和使用遥测数据，如 Watson。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2d2cc8c0705826015db58ab184b8a499fa2b9c00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530100"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="812f1-103">diagnosticDataSubmissionMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="812f1-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="812f1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="812f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="812f1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="812f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="812f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="812f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="812f1-107">允许设备发送诊断和使用遥测数据，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="812f1-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="812f1-108">成员</span><span class="sxs-lookup"><span data-stu-id="812f1-108">Members</span></span>
|<span data-ttu-id="812f1-109">成员</span><span class="sxs-lookup"><span data-stu-id="812f1-109">Member</span></span>|<span data-ttu-id="812f1-110">值</span><span class="sxs-lookup"><span data-stu-id="812f1-110">Value</span></span>|<span data-ttu-id="812f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="812f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="812f1-112">定制</span><span class="sxs-lookup"><span data-stu-id="812f1-112">userDefined</span></span>|<span data-ttu-id="812f1-113">0</span><span class="sxs-lookup"><span data-stu-id="812f1-113">0</span></span>|<span data-ttu-id="812f1-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="812f1-114">Allow the user to set.</span></span>|
|<span data-ttu-id="812f1-115">无</span><span class="sxs-lookup"><span data-stu-id="812f1-115">none</span></span>|<span data-ttu-id="812f1-116">1 </span><span class="sxs-lookup"><span data-stu-id="812f1-116">1</span></span>|<span data-ttu-id="812f1-117">不会从 OS 组件发送遥测数据。</span><span class="sxs-lookup"><span data-stu-id="812f1-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="812f1-118">注意：此值仅适用于企业和服务器设备。</span><span class="sxs-lookup"><span data-stu-id="812f1-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="812f1-119">在其他设备上使用此设置等效于将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="812f1-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="812f1-120">vba</span><span class="sxs-lookup"><span data-stu-id="812f1-120">basic</span></span>|<span data-ttu-id="812f1-121">2 </span><span class="sxs-lookup"><span data-stu-id="812f1-121">2</span></span>|<span data-ttu-id="812f1-122">发送基本遥测数据。</span><span class="sxs-lookup"><span data-stu-id="812f1-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="812f1-123">有所</span><span class="sxs-lookup"><span data-stu-id="812f1-123">enhanced</span></span>|<span data-ttu-id="812f1-124">3 </span><span class="sxs-lookup"><span data-stu-id="812f1-124">3</span></span>|<span data-ttu-id="812f1-125">发送包含使用率和见解数据的增强遥测数据。</span><span class="sxs-lookup"><span data-stu-id="812f1-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="812f1-126">全</span><span class="sxs-lookup"><span data-stu-id="812f1-126">full</span></span>|<span data-ttu-id="812f1-127">4 </span><span class="sxs-lookup"><span data-stu-id="812f1-127">4</span></span>|<span data-ttu-id="812f1-128">发送包含诊断数据（如系统状态）的完整遥测数据。</span><span class="sxs-lookup"><span data-stu-id="812f1-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



