---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 841917ac69bee58ac3559daf9ac4d806a069adda
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697383"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="a31e1-103">groupPolicyConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a31e1-103">groupPolicyConfigurationType enum type</span></span>

<span data-ttu-id="a31e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a31e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a31e1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a31e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a31e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a31e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a31e1-107">组策略配置类型</span><span class="sxs-lookup"><span data-stu-id="a31e1-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="a31e1-108">成员</span><span class="sxs-lookup"><span data-stu-id="a31e1-108">Members</span></span>
|<span data-ttu-id="a31e1-109">成员</span><span class="sxs-lookup"><span data-stu-id="a31e1-109">Member</span></span>|<span data-ttu-id="a31e1-110">值</span><span class="sxs-lookup"><span data-stu-id="a31e1-110">Value</span></span>|<span data-ttu-id="a31e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="a31e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a31e1-112">策略</span><span class="sxs-lookup"><span data-stu-id="a31e1-112">policy</span></span>|<span data-ttu-id="a31e1-113">0</span><span class="sxs-lookup"><span data-stu-id="a31e1-113">0</span></span>|<span data-ttu-id="a31e1-114">策略类型不 tattoo 值，这意味着将删除值，允许使用原始配置值。</span><span class="sxs-lookup"><span data-stu-id="a31e1-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="a31e1-115">策略类型取代应用程序配置设置，以便应用程序始终知道该值。</span><span class="sxs-lookup"><span data-stu-id="a31e1-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="a31e1-116">策略类型可阻止用户通过应用程序的用户界面修改值。</span><span class="sxs-lookup"><span data-stu-id="a31e1-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="a31e1-117">优先权</span><span class="sxs-lookup"><span data-stu-id="a31e1-117">preference</span></span>|<span data-ttu-id="a31e1-118">1</span><span class="sxs-lookup"><span data-stu-id="a31e1-118">1</span></span>|<span data-ttu-id="a31e1-119">首选项类型不 tattoo 值，这意味着不会从注册表中删除该值。</span><span class="sxs-lookup"><span data-stu-id="a31e1-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="a31e1-120">首选项类型将覆盖用户配置的值，并且不会保留以前的值。</span><span class="sxs-lookup"><span data-stu-id="a31e1-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="a31e1-121">首选类型不阻止用户通过应用程序的用户界面修改值。</span><span class="sxs-lookup"><span data-stu-id="a31e1-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





