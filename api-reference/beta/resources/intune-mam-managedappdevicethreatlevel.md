---
title: managedAppDeviceThreatLevel 枚举类型
description: 允许应用程序兼容的 maxium 威胁级别。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a676a27abeb48bd5a6cc487e036fa08db3afcda
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538873"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="f1a01-103">managedAppDeviceThreatLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f1a01-103">managedAppDeviceThreatLevel enum type</span></span>

> <span data-ttu-id="f1a01-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1a01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a01-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1a01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a01-106">允许应用程序兼容的 maxium 威胁级别。</span><span class="sxs-lookup"><span data-stu-id="f1a01-106">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="f1a01-107">成员</span><span class="sxs-lookup"><span data-stu-id="f1a01-107">Members</span></span>
|<span data-ttu-id="f1a01-108">成员</span><span class="sxs-lookup"><span data-stu-id="f1a01-108">Member</span></span>|<span data-ttu-id="f1a01-109">值</span><span class="sxs-lookup"><span data-stu-id="f1a01-109">Value</span></span>|<span data-ttu-id="f1a01-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1a01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a01-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f1a01-111">notConfigured</span></span>|<span data-ttu-id="f1a01-112">0</span><span class="sxs-lookup"><span data-stu-id="f1a01-112">0</span></span>|<span data-ttu-id="f1a01-113">未配置值</span><span class="sxs-lookup"><span data-stu-id="f1a01-113">Value not configured</span></span>|
|<span data-ttu-id="f1a01-114">加密</span><span class="sxs-lookup"><span data-stu-id="f1a01-114">secured</span></span>|<span data-ttu-id="f1a01-115">1</span><span class="sxs-lookup"><span data-stu-id="f1a01-115">1</span></span>|<span data-ttu-id="f1a01-116">设备需要无威胁</span><span class="sxs-lookup"><span data-stu-id="f1a01-116">Device needs to have no threat</span></span>|
|<span data-ttu-id="f1a01-117">降低</span><span class="sxs-lookup"><span data-stu-id="f1a01-117">low</span></span>|<span data-ttu-id="f1a01-118">双面</span><span class="sxs-lookup"><span data-stu-id="f1a01-118">2</span></span>|<span data-ttu-id="f1a01-119">设备需要较低的威胁。</span><span class="sxs-lookup"><span data-stu-id="f1a01-119">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="f1a01-120">中等</span><span class="sxs-lookup"><span data-stu-id="f1a01-120">medium</span></span>|<span data-ttu-id="f1a01-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f1a01-121">3</span></span>|<span data-ttu-id="f1a01-122">设备需要的威胁不超过中型威胁。</span><span class="sxs-lookup"><span data-stu-id="f1a01-122">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="f1a01-123">高效</span><span class="sxs-lookup"><span data-stu-id="f1a01-123">high</span></span>|<span data-ttu-id="f1a01-124">4 </span><span class="sxs-lookup"><span data-stu-id="f1a01-124">4</span></span>|<span data-ttu-id="f1a01-125">设备需要的威胁不超过高</span><span class="sxs-lookup"><span data-stu-id="f1a01-125">Device needs to have not more than high threat</span></span>|



