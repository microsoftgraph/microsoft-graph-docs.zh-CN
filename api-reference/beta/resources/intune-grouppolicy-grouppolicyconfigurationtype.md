---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6e0e7f2b1a9c7817af614c2753e4e5fcfe0fe2c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011006"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="2d521-103">groupPolicyConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2d521-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="2d521-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d521-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d521-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d521-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d521-106">组策略配置类型</span><span class="sxs-lookup"><span data-stu-id="2d521-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="2d521-107">成员</span><span class="sxs-lookup"><span data-stu-id="2d521-107">Members</span></span>
|<span data-ttu-id="2d521-108">成员</span><span class="sxs-lookup"><span data-stu-id="2d521-108">Member</span></span>|<span data-ttu-id="2d521-109">值</span><span class="sxs-lookup"><span data-stu-id="2d521-109">Value</span></span>|<span data-ttu-id="2d521-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d521-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d521-111">policy</span><span class="sxs-lookup"><span data-stu-id="2d521-111">policy</span></span>|<span data-ttu-id="2d521-112">0</span><span class="sxs-lookup"><span data-stu-id="2d521-112">0</span></span>|<span data-ttu-id="2d521-113">策略类型不 tattoo 值, 这意味着将删除值, 允许使用原始配置值。</span><span class="sxs-lookup"><span data-stu-id="2d521-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="2d521-114">策略类型取代应用程序配置设置, 以便应用程序始终知道该值。</span><span class="sxs-lookup"><span data-stu-id="2d521-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="2d521-115">策略类型可阻止用户通过应用程序的用户界面修改值。</span><span class="sxs-lookup"><span data-stu-id="2d521-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="2d521-116">优先权</span><span class="sxs-lookup"><span data-stu-id="2d521-116">preference</span></span>|<span data-ttu-id="2d521-117">1</span><span class="sxs-lookup"><span data-stu-id="2d521-117">1</span></span>|<span data-ttu-id="2d521-118">首选项类型不 tattoo 值, 这意味着不会从注册表中删除该值。</span><span class="sxs-lookup"><span data-stu-id="2d521-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="2d521-119">首选项类型将覆盖用户配置的值, 并且不会保留以前的值。</span><span class="sxs-lookup"><span data-stu-id="2d521-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="2d521-120">首选类型不阻止用户通过应用程序的用户界面修改值。</span><span class="sxs-lookup"><span data-stu-id="2d521-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





