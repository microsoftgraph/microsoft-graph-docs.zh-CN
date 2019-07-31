---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a5589307692f6287301722ba67e54e7df0347f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010586"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="1e58e-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1e58e-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="1e58e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e58e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e58e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e58e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e58e-106">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="1e58e-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="1e58e-107">成员</span><span class="sxs-lookup"><span data-stu-id="1e58e-107">Members</span></span>
|<span data-ttu-id="1e58e-108">成员</span><span class="sxs-lookup"><span data-stu-id="1e58e-108">Member</span></span>|<span data-ttu-id="1e58e-109">值</span><span class="sxs-lookup"><span data-stu-id="1e58e-109">Value</span></span>|<span data-ttu-id="1e58e-110">说明</span><span class="sxs-lookup"><span data-stu-id="1e58e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e58e-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="1e58e-111">resourceScope</span></span>|<span data-ttu-id="1e58e-112">0</span><span class="sxs-lookup"><span data-stu-id="1e58e-112">0</span></span>|<span data-ttu-id="1e58e-113">允许分配给指定的 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="1e58e-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="1e58e-114">allDevices</span><span class="sxs-lookup"><span data-stu-id="1e58e-114">allDevices</span></span>|<span data-ttu-id="1e58e-115">1</span><span class="sxs-lookup"><span data-stu-id="1e58e-115">1</span></span>|<span data-ttu-id="1e58e-116">允许向所有 Intune 设备分配作业。</span><span class="sxs-lookup"><span data-stu-id="1e58e-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="1e58e-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="1e58e-117">allLicensedUsers</span></span>|<span data-ttu-id="1e58e-118">双面</span><span class="sxs-lookup"><span data-stu-id="1e58e-118">2</span></span>|<span data-ttu-id="1e58e-119">允许向所有 Intune 许可用户分配作业。</span><span class="sxs-lookup"><span data-stu-id="1e58e-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="1e58e-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="1e58e-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="1e58e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="1e58e-121">3</span></span>|<span data-ttu-id="1e58e-122">允许分配给所有 Intune 设备和许可的用户。</span><span class="sxs-lookup"><span data-stu-id="1e58e-122">Allow assignments to all Intune devices and licensed users.</span></span>|





