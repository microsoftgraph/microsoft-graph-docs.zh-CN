---
title: enrollmentAvailabilityOptions 枚举类型
description: 可用于注册流自定义的选项
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef3f853a94ca8cdf902668acd512e66b10519909
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162391"
---
# <a name="enrollmentavailabilityoptions-enum-type"></a><span data-ttu-id="9da83-103">enrollmentAvailabilityOptions 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9da83-103">enrollmentAvailabilityOptions enum type</span></span>

> <span data-ttu-id="9da83-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9da83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9da83-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9da83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9da83-106">可用于注册流自定义的选项</span><span class="sxs-lookup"><span data-stu-id="9da83-106">Options available for enrollment flow customization</span></span>

## <a name="members"></a><span data-ttu-id="9da83-107">成员</span><span class="sxs-lookup"><span data-stu-id="9da83-107">Members</span></span>
|<span data-ttu-id="9da83-108">成员</span><span class="sxs-lookup"><span data-stu-id="9da83-108">Member</span></span>|<span data-ttu-id="9da83-109">值</span><span class="sxs-lookup"><span data-stu-id="9da83-109">Value</span></span>|<span data-ttu-id="9da83-110">说明</span><span class="sxs-lookup"><span data-stu-id="9da83-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9da83-111">availableWithPrompts</span><span class="sxs-lookup"><span data-stu-id="9da83-111">availableWithPrompts</span></span>|<span data-ttu-id="9da83-112">0</span><span class="sxs-lookup"><span data-stu-id="9da83-112">0</span></span>|<span data-ttu-id="9da83-113">使用引导注册提示向最终用户显示设备注册流</span><span class="sxs-lookup"><span data-stu-id="9da83-113">Device enrollment flow is shown to the end user with guided enrollment prompts</span></span>|
|<span data-ttu-id="9da83-114">availableWithoutPrompts</span><span class="sxs-lookup"><span data-stu-id="9da83-114">availableWithoutPrompts</span></span>|<span data-ttu-id="9da83-115">1</span><span class="sxs-lookup"><span data-stu-id="9da83-115">1</span></span>|<span data-ttu-id="9da83-116">没有引导注册提示的最终用户可以使用设备注册流</span><span class="sxs-lookup"><span data-stu-id="9da83-116">Device enrollment flow is available to the end user without guided enrollment prompts</span></span>|
|<span data-ttu-id="9da83-117">才</span><span class="sxs-lookup"><span data-stu-id="9da83-117">unavailable</span></span>|<span data-ttu-id="9da83-118">双面</span><span class="sxs-lookup"><span data-stu-id="9da83-118">2</span></span>|<span data-ttu-id="9da83-119">设备注册流对 enduser 不可用</span><span class="sxs-lookup"><span data-stu-id="9da83-119">Device enrollment flow is unavailable to the enduser</span></span>|



