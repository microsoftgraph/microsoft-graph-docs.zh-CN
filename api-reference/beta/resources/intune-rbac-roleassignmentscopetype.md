---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573051"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="793b7-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="793b7-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="793b7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="793b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="793b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="793b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="793b7-106">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="793b7-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="793b7-107">成员</span><span class="sxs-lookup"><span data-stu-id="793b7-107">Members</span></span>
|<span data-ttu-id="793b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="793b7-108">Member</span></span>|<span data-ttu-id="793b7-109">值</span><span class="sxs-lookup"><span data-stu-id="793b7-109">Value</span></span>|<span data-ttu-id="793b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="793b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="793b7-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="793b7-111">resourceScope</span></span>|<span data-ttu-id="793b7-112">0</span><span class="sxs-lookup"><span data-stu-id="793b7-112">0</span></span>|<span data-ttu-id="793b7-113">允许分配给指定的 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="793b7-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="793b7-114">allDevices</span><span class="sxs-lookup"><span data-stu-id="793b7-114">allDevices</span></span>|<span data-ttu-id="793b7-115">1</span><span class="sxs-lookup"><span data-stu-id="793b7-115">1</span></span>|<span data-ttu-id="793b7-116">允许向所有 Intune 设备分配作业。</span><span class="sxs-lookup"><span data-stu-id="793b7-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="793b7-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="793b7-117">allLicensedUsers</span></span>|<span data-ttu-id="793b7-118">2 </span><span class="sxs-lookup"><span data-stu-id="793b7-118">2</span></span>|<span data-ttu-id="793b7-119">允许向所有 Intune 许可用户分配作业。</span><span class="sxs-lookup"><span data-stu-id="793b7-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="793b7-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="793b7-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="793b7-121">3 </span><span class="sxs-lookup"><span data-stu-id="793b7-121">3</span></span>|<span data-ttu-id="793b7-122">允许分配给所有 Intune 设备和许可的用户。</span><span class="sxs-lookup"><span data-stu-id="793b7-122">Allow assignments to all Intune devices and licensed users.</span></span>|





