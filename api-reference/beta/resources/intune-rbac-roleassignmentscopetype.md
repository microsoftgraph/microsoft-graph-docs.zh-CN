---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3205b3ffb451f6ab62e7573e94a4347491a0c7cb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259135"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="075b1-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="075b1-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="075b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="075b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="075b1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="075b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="075b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="075b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="075b1-107">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="075b1-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="075b1-108">成员</span><span class="sxs-lookup"><span data-stu-id="075b1-108">Members</span></span>
|<span data-ttu-id="075b1-109">成员</span><span class="sxs-lookup"><span data-stu-id="075b1-109">Member</span></span>|<span data-ttu-id="075b1-110">值</span><span class="sxs-lookup"><span data-stu-id="075b1-110">Value</span></span>|<span data-ttu-id="075b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="075b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="075b1-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="075b1-112">resourceScope</span></span>|<span data-ttu-id="075b1-113">0</span><span class="sxs-lookup"><span data-stu-id="075b1-113">0</span></span>|<span data-ttu-id="075b1-114">允许分配给指定的 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="075b1-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="075b1-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="075b1-115">allDevices</span></span>|<span data-ttu-id="075b1-116">1</span><span class="sxs-lookup"><span data-stu-id="075b1-116">1</span></span>|<span data-ttu-id="075b1-117">允许向所有 Intune 设备分配作业。</span><span class="sxs-lookup"><span data-stu-id="075b1-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="075b1-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="075b1-118">allLicensedUsers</span></span>|<span data-ttu-id="075b1-119">双面</span><span class="sxs-lookup"><span data-stu-id="075b1-119">2</span></span>|<span data-ttu-id="075b1-120">允许向所有 Intune 许可用户分配作业。</span><span class="sxs-lookup"><span data-stu-id="075b1-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="075b1-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="075b1-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="075b1-122">第三章</span><span class="sxs-lookup"><span data-stu-id="075b1-122">3</span></span>|<span data-ttu-id="075b1-123">允许分配给所有 Intune 设备和许可的用户。</span><span class="sxs-lookup"><span data-stu-id="075b1-123">Allow assignments to all Intune devices and licensed users.</span></span>|




