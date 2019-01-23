---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429410"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="f1c86-103">groupPolicyConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f1c86-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="f1c86-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f1c86-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1c86-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1c86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1c86-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1c86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1c86-107">组策略配置类型</span><span class="sxs-lookup"><span data-stu-id="f1c86-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="f1c86-108">成员</span><span class="sxs-lookup"><span data-stu-id="f1c86-108">Members</span></span>
|<span data-ttu-id="f1c86-109">成员</span><span class="sxs-lookup"><span data-stu-id="f1c86-109">Member</span></span>|<span data-ttu-id="f1c86-110">值</span><span class="sxs-lookup"><span data-stu-id="f1c86-110">Value</span></span>|<span data-ttu-id="f1c86-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1c86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c86-112">策略</span><span class="sxs-lookup"><span data-stu-id="f1c86-112">policy</span></span>|<span data-ttu-id="f1c86-113">0</span><span class="sxs-lookup"><span data-stu-id="f1c86-113">0</span></span>|<span data-ttu-id="f1c86-114">策略类型不图案的值，这意味着值删除允许使用的原始配置值。</span><span class="sxs-lookup"><span data-stu-id="f1c86-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="f1c86-115">策略类型取代应用程序配置设置，以便应用程序始终会知道的值。</span><span class="sxs-lookup"><span data-stu-id="f1c86-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="f1c86-116">策略类型可防止用户修改通过应用程序的用户界面的值。</span><span class="sxs-lookup"><span data-stu-id="f1c86-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="f1c86-117">preference</span><span class="sxs-lookup"><span data-stu-id="f1c86-117">preference</span></span>|<span data-ttu-id="f1c86-118">1</span><span class="sxs-lookup"><span data-stu-id="f1c86-118">1</span></span>|<span data-ttu-id="f1c86-119">首选项类型图案的值，这意味着值不从注册表中删除。</span><span class="sxs-lookup"><span data-stu-id="f1c86-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="f1c86-120">首选项类型将覆盖用户配置值并不会保留以前的值。</span><span class="sxs-lookup"><span data-stu-id="f1c86-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="f1c86-121">首选项类型不阻止用户修改通过应用程序的用户界面的值。</span><span class="sxs-lookup"><span data-stu-id="f1c86-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




