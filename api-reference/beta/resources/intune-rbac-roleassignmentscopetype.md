---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775686"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="121a0-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="121a0-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="121a0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="121a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="121a0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="121a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="121a0-106">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="121a0-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="121a0-107">成员</span><span class="sxs-lookup"><span data-stu-id="121a0-107">Members</span></span>
|<span data-ttu-id="121a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="121a0-108">Member</span></span>|<span data-ttu-id="121a0-109">值</span><span class="sxs-lookup"><span data-stu-id="121a0-109">Value</span></span>|<span data-ttu-id="121a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="121a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="121a0-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="121a0-111">resourceScope</span></span>|<span data-ttu-id="121a0-112">0</span><span class="sxs-lookup"><span data-stu-id="121a0-112">0</span></span>|<span data-ttu-id="121a0-113">允许分配给指定的 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="121a0-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="121a0-114">allDevices</span><span class="sxs-lookup"><span data-stu-id="121a0-114">allDevices</span></span>|<span data-ttu-id="121a0-115">1</span><span class="sxs-lookup"><span data-stu-id="121a0-115">1</span></span>|<span data-ttu-id="121a0-116">允许向所有 Intune 设备分配作业。</span><span class="sxs-lookup"><span data-stu-id="121a0-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="121a0-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="121a0-117">allLicensedUsers</span></span>|<span data-ttu-id="121a0-118">双面</span><span class="sxs-lookup"><span data-stu-id="121a0-118">2</span></span>|<span data-ttu-id="121a0-119">允许向所有 Intune 许可用户分配作业。</span><span class="sxs-lookup"><span data-stu-id="121a0-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="121a0-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="121a0-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="121a0-121">第三章</span><span class="sxs-lookup"><span data-stu-id="121a0-121">3</span></span>|<span data-ttu-id="121a0-122">允许分配给所有 Intune 设备和许可的用户。</span><span class="sxs-lookup"><span data-stu-id="121a0-122">Allow assignments to all Intune devices and licensed users.</span></span>|





