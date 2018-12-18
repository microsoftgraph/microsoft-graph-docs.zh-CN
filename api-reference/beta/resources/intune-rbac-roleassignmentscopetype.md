---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: tfitzmac
ms.openlocfilehash: 0a3286b3b7bc583323204ca39ff85e01869ddbe7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343125"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="49b71-103">roleAssignmentScopeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49b71-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="49b71-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49b71-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49b71-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49b71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49b71-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49b71-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49b71-107">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="49b71-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="49b71-108">成员</span><span class="sxs-lookup"><span data-stu-id="49b71-108">Members</span></span>
|<span data-ttu-id="49b71-109">成员</span><span class="sxs-lookup"><span data-stu-id="49b71-109">Member</span></span>|<span data-ttu-id="49b71-110">值</span><span class="sxs-lookup"><span data-stu-id="49b71-110">Value</span></span>|<span data-ttu-id="49b71-111">说明</span><span class="sxs-lookup"><span data-stu-id="49b71-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49b71-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="49b71-112">resourceScope</span></span>|<span data-ttu-id="49b71-113">0</span><span class="sxs-lookup"><span data-stu-id="49b71-113">0</span></span>|<span data-ttu-id="49b71-114">允许分配给指定 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="49b71-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="49b71-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="49b71-115">allDevices</span></span>|<span data-ttu-id="49b71-116">1</span><span class="sxs-lookup"><span data-stu-id="49b71-116">1</span></span>|<span data-ttu-id="49b71-117">允许分配给所有 Intune 设备。</span><span class="sxs-lookup"><span data-stu-id="49b71-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="49b71-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="49b71-118">allLicensedUsers</span></span>|<span data-ttu-id="49b71-119">2</span><span class="sxs-lookup"><span data-stu-id="49b71-119">2</span></span>|<span data-ttu-id="49b71-120">允许分配给所有 Intune 授权用户。</span><span class="sxs-lookup"><span data-stu-id="49b71-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="49b71-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="49b71-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="49b71-122">3</span><span class="sxs-lookup"><span data-stu-id="49b71-122">3</span></span>|<span data-ttu-id="49b71-123">允许分配给所有 Intune 设备和授权的用户。</span><span class="sxs-lookup"><span data-stu-id="49b71-123">Allow assignments to all Intune devices and licensed users.</span></span>|





