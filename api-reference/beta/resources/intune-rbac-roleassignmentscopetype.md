---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419889"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="ecb4a-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ecb4a-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="ecb4a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ecb4a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecb4a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecb4a-107">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="ecb4a-108">成员</span><span class="sxs-lookup"><span data-stu-id="ecb4a-108">Members</span></span>
|<span data-ttu-id="ecb4a-109">成员</span><span class="sxs-lookup"><span data-stu-id="ecb4a-109">Member</span></span>|<span data-ttu-id="ecb4a-110">值</span><span class="sxs-lookup"><span data-stu-id="ecb4a-110">Value</span></span>|<span data-ttu-id="ecb4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ecb4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecb4a-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="ecb4a-112">resourceScope</span></span>|<span data-ttu-id="ecb4a-113">0</span><span class="sxs-lookup"><span data-stu-id="ecb4a-113">0</span></span>|<span data-ttu-id="ecb4a-114">允许分配给指定 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="ecb4a-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="ecb4a-115">allDevices</span></span>|<span data-ttu-id="ecb4a-116">1</span><span class="sxs-lookup"><span data-stu-id="ecb4a-116">1</span></span>|<span data-ttu-id="ecb4a-117">允许分配给所有 Intune 设备。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="ecb4a-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="ecb4a-118">allLicensedUsers</span></span>|<span data-ttu-id="ecb4a-119">2</span><span class="sxs-lookup"><span data-stu-id="ecb4a-119">2</span></span>|<span data-ttu-id="ecb4a-120">允许分配给所有 Intune 授权用户。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="ecb4a-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="ecb4a-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="ecb4a-122">3</span><span class="sxs-lookup"><span data-stu-id="ecb4a-122">3</span></span>|<span data-ttu-id="ecb4a-123">允许分配给所有 Intune 设备和授权的用户。</span><span class="sxs-lookup"><span data-stu-id="ecb4a-123">Allow assignments to all Intune devices and licensed users.</span></span>|




