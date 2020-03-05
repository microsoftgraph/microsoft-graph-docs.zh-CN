---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f922cf51729f178ab9ca94db127efb5b70bb94fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523891"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="9c88e-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9c88e-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="9c88e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9c88e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c88e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c88e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c88e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c88e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c88e-107">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="9c88e-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="9c88e-108">成员</span><span class="sxs-lookup"><span data-stu-id="9c88e-108">Members</span></span>
|<span data-ttu-id="9c88e-109">成员</span><span class="sxs-lookup"><span data-stu-id="9c88e-109">Member</span></span>|<span data-ttu-id="9c88e-110">值</span><span class="sxs-lookup"><span data-stu-id="9c88e-110">Value</span></span>|<span data-ttu-id="9c88e-111">说明</span><span class="sxs-lookup"><span data-stu-id="9c88e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c88e-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="9c88e-112">resourceScope</span></span>|<span data-ttu-id="9c88e-113">0</span><span class="sxs-lookup"><span data-stu-id="9c88e-113">0</span></span>|<span data-ttu-id="9c88e-114">允许分配给指定的 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="9c88e-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="9c88e-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="9c88e-115">allDevices</span></span>|<span data-ttu-id="9c88e-116">1 </span><span class="sxs-lookup"><span data-stu-id="9c88e-116">1</span></span>|<span data-ttu-id="9c88e-117">允许向所有 Intune 设备分配作业。</span><span class="sxs-lookup"><span data-stu-id="9c88e-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="9c88e-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="9c88e-118">allLicensedUsers</span></span>|<span data-ttu-id="9c88e-119">2 </span><span class="sxs-lookup"><span data-stu-id="9c88e-119">2</span></span>|<span data-ttu-id="9c88e-120">允许向所有 Intune 许可用户分配作业。</span><span class="sxs-lookup"><span data-stu-id="9c88e-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="9c88e-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="9c88e-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="9c88e-122">3 </span><span class="sxs-lookup"><span data-stu-id="9c88e-122">3</span></span>|<span data-ttu-id="9c88e-123">允许分配给所有 Intune 设备和许可的用户。</span><span class="sxs-lookup"><span data-stu-id="9c88e-123">Allow assignments to all Intune devices and licensed users.</span></span>|



