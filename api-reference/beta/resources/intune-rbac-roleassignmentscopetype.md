---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a88fc1f8976e9d87c166cab2ebde865f049ed91b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43357301"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="f5e6d-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5e6d-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="f5e6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5e6d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5e6d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5e6d-107">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="f5e6d-108">成员</span><span class="sxs-lookup"><span data-stu-id="f5e6d-108">Members</span></span>
|<span data-ttu-id="f5e6d-109">成员</span><span class="sxs-lookup"><span data-stu-id="f5e6d-109">Member</span></span>|<span data-ttu-id="f5e6d-110">值</span><span class="sxs-lookup"><span data-stu-id="f5e6d-110">Value</span></span>|<span data-ttu-id="f5e6d-111">说明</span><span class="sxs-lookup"><span data-stu-id="f5e6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5e6d-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="f5e6d-112">resourceScope</span></span>|<span data-ttu-id="f5e6d-113">0</span><span class="sxs-lookup"><span data-stu-id="f5e6d-113">0</span></span>|<span data-ttu-id="f5e6d-114">允许分配给指定的 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="f5e6d-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="f5e6d-115">allDevices</span></span>|<span data-ttu-id="f5e6d-116">1</span><span class="sxs-lookup"><span data-stu-id="f5e6d-116">1</span></span>|<span data-ttu-id="f5e6d-117">允许向所有 Intune 设备分配作业。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="f5e6d-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="f5e6d-118">allLicensedUsers</span></span>|<span data-ttu-id="f5e6d-119">双面</span><span class="sxs-lookup"><span data-stu-id="f5e6d-119">2</span></span>|<span data-ttu-id="f5e6d-120">允许向所有 Intune 许可用户分配作业。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="f5e6d-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="f5e6d-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="f5e6d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f5e6d-122">3</span></span>|<span data-ttu-id="f5e6d-123">允许分配给所有 Intune 设备和许可的用户。</span><span class="sxs-lookup"><span data-stu-id="f5e6d-123">Allow assignments to all Intune devices and licensed users.</span></span>|



