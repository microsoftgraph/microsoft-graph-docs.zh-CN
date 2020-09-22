---
title: enrollmentAvailabilityOptions 枚举类型
description: 可用于注册流自定义的选项
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 10204def9d2952a092f6453f1a15c9be2d745366
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084301"
---
# <a name="enrollmentavailabilityoptions-enum-type"></a><span data-ttu-id="63735-103">enrollmentAvailabilityOptions 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63735-103">enrollmentAvailabilityOptions enum type</span></span>

<span data-ttu-id="63735-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63735-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63735-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63735-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63735-107">可用于注册流自定义的选项</span><span class="sxs-lookup"><span data-stu-id="63735-107">Options available for enrollment flow customization</span></span>

## <a name="members"></a><span data-ttu-id="63735-108">成员</span><span class="sxs-lookup"><span data-stu-id="63735-108">Members</span></span>
|<span data-ttu-id="63735-109">成员</span><span class="sxs-lookup"><span data-stu-id="63735-109">Member</span></span>|<span data-ttu-id="63735-110">值</span><span class="sxs-lookup"><span data-stu-id="63735-110">Value</span></span>|<span data-ttu-id="63735-111">说明</span><span class="sxs-lookup"><span data-stu-id="63735-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63735-112">availableWithPrompts</span><span class="sxs-lookup"><span data-stu-id="63735-112">availableWithPrompts</span></span>|<span data-ttu-id="63735-113">0</span><span class="sxs-lookup"><span data-stu-id="63735-113">0</span></span>|<span data-ttu-id="63735-114">使用引导注册提示向最终用户显示设备注册流</span><span class="sxs-lookup"><span data-stu-id="63735-114">Device enrollment flow is shown to the end user with guided enrollment prompts</span></span>|
|<span data-ttu-id="63735-115">availableWithoutPrompts</span><span class="sxs-lookup"><span data-stu-id="63735-115">availableWithoutPrompts</span></span>|<span data-ttu-id="63735-116">1 </span><span class="sxs-lookup"><span data-stu-id="63735-116">1</span></span>|<span data-ttu-id="63735-117">没有引导注册提示的最终用户可以使用设备注册流</span><span class="sxs-lookup"><span data-stu-id="63735-117">Device enrollment flow is available to the end user without guided enrollment prompts</span></span>|
|<span data-ttu-id="63735-118">才</span><span class="sxs-lookup"><span data-stu-id="63735-118">unavailable</span></span>|<span data-ttu-id="63735-119">2 </span><span class="sxs-lookup"><span data-stu-id="63735-119">2</span></span>|<span data-ttu-id="63735-120">设备注册流对 enduser 不可用</span><span class="sxs-lookup"><span data-stu-id="63735-120">Device enrollment flow is unavailable to the enduser</span></span>|






