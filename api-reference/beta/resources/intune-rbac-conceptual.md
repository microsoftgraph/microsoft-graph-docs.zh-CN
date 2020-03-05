---
title: Microsoft Intune 中的基于角色的访问控制
description: 列出用于定义和管理租户组织的基于角色的访问控制（RBAC）的 Intune 终结点（REST）的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 86f0e3c08bf1180969085d49f715cc6c52d8aec4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527569"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="9db85-103">Microsoft Intune 中的基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="9db85-103">Role-based access control in Microsoft Intune</span></span>

<span data-ttu-id="9db85-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9db85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9db85-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9db85-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9db85-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9db85-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9db85-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9db85-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9db85-108">Intune 的基于角色的访问控制决定哪些人可以对 Intune 对象执行操作并可更改托管应用程序、用户和设备。</span><span class="sxs-lookup"><span data-stu-id="9db85-108">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="9db85-109">以下 Graph 资源可用于管理 Intune 中基于角色的访问控制：</span><span class="sxs-lookup"><span data-stu-id="9db85-109">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="9db85-110">设备和应用管理分配的角色详情</span><span class="sxs-lookup"><span data-stu-id="9db85-110">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="9db85-111">设备和应用管理角色分配</span><span class="sxs-lookup"><span data-stu-id="9db85-111">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="9db85-112">设备和应用管理角色定义</span><span class="sxs-lookup"><span data-stu-id="9db85-112">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="9db85-113">资源操作</span><span class="sxs-lookup"><span data-stu-id="9db85-113">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="9db85-114">资源操作</span><span class="sxs-lookup"><span data-stu-id="9db85-114">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="9db85-115">角色分配</span><span class="sxs-lookup"><span data-stu-id="9db85-115">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="9db85-116">角色分配范围类型</span><span class="sxs-lookup"><span data-stu-id="9db85-116">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="9db85-117">角色定义</span><span class="sxs-lookup"><span data-stu-id="9db85-117">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="9db85-118">角色权限</span><span class="sxs-lookup"><span data-stu-id="9db85-118">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="9db85-119">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="9db85-119">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="9db85-120">角色作用域标记自动分配</span><span class="sxs-lookup"><span data-stu-id="9db85-120">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)
