---
title: managedAppDeviceThreatLevel 枚举类型
description: 允许应用程序兼容的 maxium 威胁级别。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbecc5777380d69fd1b8ca64c84637d8d5490007
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43373074"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="08639-103">managedAppDeviceThreatLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="08639-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="08639-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08639-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08639-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08639-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08639-107">允许应用程序兼容的 maxium 威胁级别。</span><span class="sxs-lookup"><span data-stu-id="08639-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="08639-108">成员</span><span class="sxs-lookup"><span data-stu-id="08639-108">Members</span></span>
|<span data-ttu-id="08639-109">成员</span><span class="sxs-lookup"><span data-stu-id="08639-109">Member</span></span>|<span data-ttu-id="08639-110">值</span><span class="sxs-lookup"><span data-stu-id="08639-110">Value</span></span>|<span data-ttu-id="08639-111">说明</span><span class="sxs-lookup"><span data-stu-id="08639-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08639-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="08639-112">notConfigured</span></span>|<span data-ttu-id="08639-113">0</span><span class="sxs-lookup"><span data-stu-id="08639-113">0</span></span>|<span data-ttu-id="08639-114">未配置值</span><span class="sxs-lookup"><span data-stu-id="08639-114">Value not configured</span></span>|
|<span data-ttu-id="08639-115">加密</span><span class="sxs-lookup"><span data-stu-id="08639-115">secured</span></span>|<span data-ttu-id="08639-116">1</span><span class="sxs-lookup"><span data-stu-id="08639-116">1</span></span>|<span data-ttu-id="08639-117">设备需要无威胁</span><span class="sxs-lookup"><span data-stu-id="08639-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="08639-118">降低</span><span class="sxs-lookup"><span data-stu-id="08639-118">low</span></span>|<span data-ttu-id="08639-119">双面</span><span class="sxs-lookup"><span data-stu-id="08639-119">2</span></span>|<span data-ttu-id="08639-120">设备需要较低的威胁。</span><span class="sxs-lookup"><span data-stu-id="08639-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="08639-121">中等</span><span class="sxs-lookup"><span data-stu-id="08639-121">medium</span></span>|<span data-ttu-id="08639-122">第三章</span><span class="sxs-lookup"><span data-stu-id="08639-122">3</span></span>|<span data-ttu-id="08639-123">设备需要的威胁不超过中型威胁。</span><span class="sxs-lookup"><span data-stu-id="08639-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="08639-124">高效</span><span class="sxs-lookup"><span data-stu-id="08639-124">high</span></span>|<span data-ttu-id="08639-125">4 </span><span class="sxs-lookup"><span data-stu-id="08639-125">4</span></span>|<span data-ttu-id="08639-126">设备需要的威胁不超过高</span><span class="sxs-lookup"><span data-stu-id="08639-126">Device needs to have not more than high threat</span></span>|



