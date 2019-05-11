---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0de9f7c08aede2e4533c22f087884801ee2c3855
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941147"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="964a3-103">groupPolicyConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="964a3-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="964a3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="964a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="964a3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="964a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="964a3-106">组策略配置类型</span><span class="sxs-lookup"><span data-stu-id="964a3-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="964a3-107">成员</span><span class="sxs-lookup"><span data-stu-id="964a3-107">Members</span></span>
|<span data-ttu-id="964a3-108">成员</span><span class="sxs-lookup"><span data-stu-id="964a3-108">Member</span></span>|<span data-ttu-id="964a3-109">值</span><span class="sxs-lookup"><span data-stu-id="964a3-109">Value</span></span>|<span data-ttu-id="964a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="964a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="964a3-111">policy</span><span class="sxs-lookup"><span data-stu-id="964a3-111">policy</span></span>|<span data-ttu-id="964a3-112">0</span><span class="sxs-lookup"><span data-stu-id="964a3-112">0</span></span>|<span data-ttu-id="964a3-113">策略类型不 tattoo 值, 这意味着将删除值, 允许使用原始配置值。</span><span class="sxs-lookup"><span data-stu-id="964a3-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="964a3-114">策略类型取代应用程序配置设置, 以便应用程序始终知道该值。</span><span class="sxs-lookup"><span data-stu-id="964a3-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="964a3-115">策略类型可阻止用户通过应用程序的用户界面修改值。</span><span class="sxs-lookup"><span data-stu-id="964a3-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="964a3-116">优先权</span><span class="sxs-lookup"><span data-stu-id="964a3-116">preference</span></span>|<span data-ttu-id="964a3-117">1</span><span class="sxs-lookup"><span data-stu-id="964a3-117">1</span></span>|<span data-ttu-id="964a3-118">首选项类型不 tattoo 值, 这意味着不会从注册表中删除该值。</span><span class="sxs-lookup"><span data-stu-id="964a3-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="964a3-119">首选项类型将覆盖用户配置的值, 并且不会保留以前的值。</span><span class="sxs-lookup"><span data-stu-id="964a3-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="964a3-120">首选类型不阻止用户通过应用程序的用户界面修改值。</span><span class="sxs-lookup"><span data-stu-id="964a3-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




