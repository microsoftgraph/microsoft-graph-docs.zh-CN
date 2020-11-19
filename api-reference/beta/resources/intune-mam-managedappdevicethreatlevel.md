---
title: managedAppDeviceThreatLevel 枚举类型
description: 允许应用程序兼容的 maxium 威胁级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f262c53d62d791e456edcd234249448e0c90580c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266912"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="b443c-103">managedAppDeviceThreatLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b443c-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="b443c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b443c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b443c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b443c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b443c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b443c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b443c-107">允许应用程序兼容的 maxium 威胁级别。</span><span class="sxs-lookup"><span data-stu-id="b443c-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="b443c-108">成员</span><span class="sxs-lookup"><span data-stu-id="b443c-108">Members</span></span>
|<span data-ttu-id="b443c-109">成员</span><span class="sxs-lookup"><span data-stu-id="b443c-109">Member</span></span>|<span data-ttu-id="b443c-110">值</span><span class="sxs-lookup"><span data-stu-id="b443c-110">Value</span></span>|<span data-ttu-id="b443c-111">说明</span><span class="sxs-lookup"><span data-stu-id="b443c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b443c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b443c-112">notConfigured</span></span>|<span data-ttu-id="b443c-113">0</span><span class="sxs-lookup"><span data-stu-id="b443c-113">0</span></span>|<span data-ttu-id="b443c-114">未配置值</span><span class="sxs-lookup"><span data-stu-id="b443c-114">Value not configured</span></span>|
|<span data-ttu-id="b443c-115">加密</span><span class="sxs-lookup"><span data-stu-id="b443c-115">secured</span></span>|<span data-ttu-id="b443c-116">1</span><span class="sxs-lookup"><span data-stu-id="b443c-116">1</span></span>|<span data-ttu-id="b443c-117">设备需要无威胁</span><span class="sxs-lookup"><span data-stu-id="b443c-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="b443c-118">降低</span><span class="sxs-lookup"><span data-stu-id="b443c-118">low</span></span>|<span data-ttu-id="b443c-119">双面</span><span class="sxs-lookup"><span data-stu-id="b443c-119">2</span></span>|<span data-ttu-id="b443c-120">设备需要较低的威胁。</span><span class="sxs-lookup"><span data-stu-id="b443c-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="b443c-121">中等</span><span class="sxs-lookup"><span data-stu-id="b443c-121">medium</span></span>|<span data-ttu-id="b443c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b443c-122">3</span></span>|<span data-ttu-id="b443c-123">设备需要的威胁不超过中型威胁。</span><span class="sxs-lookup"><span data-stu-id="b443c-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="b443c-124">高效</span><span class="sxs-lookup"><span data-stu-id="b443c-124">high</span></span>|<span data-ttu-id="b443c-125">4 </span><span class="sxs-lookup"><span data-stu-id="b443c-125">4</span></span>|<span data-ttu-id="b443c-126">设备需要的威胁不超过高</span><span class="sxs-lookup"><span data-stu-id="b443c-126">Device needs to have not more than high threat</span></span>|




