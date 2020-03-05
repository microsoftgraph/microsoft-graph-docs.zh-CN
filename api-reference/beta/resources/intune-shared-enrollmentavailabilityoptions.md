---
title: enrollmentAvailabilityOptions 枚举类型
description: 可用于注册流自定义的选项
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5f4e6afaff00b200f4f085645618ef9d1e067485
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527438"
---
# <a name="enrollmentavailabilityoptions-enum-type"></a><span data-ttu-id="21029-103">enrollmentAvailabilityOptions 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21029-103">enrollmentAvailabilityOptions enum type</span></span>

<span data-ttu-id="21029-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="21029-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21029-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21029-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21029-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21029-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21029-107">可用于注册流自定义的选项</span><span class="sxs-lookup"><span data-stu-id="21029-107">Options available for enrollment flow customization</span></span>

## <a name="members"></a><span data-ttu-id="21029-108">成员</span><span class="sxs-lookup"><span data-stu-id="21029-108">Members</span></span>
|<span data-ttu-id="21029-109">成员</span><span class="sxs-lookup"><span data-stu-id="21029-109">Member</span></span>|<span data-ttu-id="21029-110">值</span><span class="sxs-lookup"><span data-stu-id="21029-110">Value</span></span>|<span data-ttu-id="21029-111">说明</span><span class="sxs-lookup"><span data-stu-id="21029-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21029-112">availableWithPrompts</span><span class="sxs-lookup"><span data-stu-id="21029-112">availableWithPrompts</span></span>|<span data-ttu-id="21029-113">0</span><span class="sxs-lookup"><span data-stu-id="21029-113">0</span></span>|<span data-ttu-id="21029-114">使用引导注册提示向最终用户显示设备注册流</span><span class="sxs-lookup"><span data-stu-id="21029-114">Device enrollment flow is shown to the end user with guided enrollment prompts</span></span>|
|<span data-ttu-id="21029-115">availableWithoutPrompts</span><span class="sxs-lookup"><span data-stu-id="21029-115">availableWithoutPrompts</span></span>|<span data-ttu-id="21029-116">1 </span><span class="sxs-lookup"><span data-stu-id="21029-116">1</span></span>|<span data-ttu-id="21029-117">没有引导注册提示的最终用户可以使用设备注册流</span><span class="sxs-lookup"><span data-stu-id="21029-117">Device enrollment flow is available to the end user without guided enrollment prompts</span></span>|
|<span data-ttu-id="21029-118">才</span><span class="sxs-lookup"><span data-stu-id="21029-118">unavailable</span></span>|<span data-ttu-id="21029-119">2 </span><span class="sxs-lookup"><span data-stu-id="21029-119">2</span></span>|<span data-ttu-id="21029-120">设备注册流对 enduser 不可用</span><span class="sxs-lookup"><span data-stu-id="21029-120">Device enrollment flow is unavailable to the enduser</span></span>|



