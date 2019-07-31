---
title: Microsoft Intune 中的基于角色的访问控制
description: 列出用于定义和管理租户组织的基于角色的访问控制 (RBAC) 的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 3f16673a2a54b4ed0de380ddd4b66aa6c74c1106
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967677"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="b70a6-103">Microsoft Intune 中的基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="b70a6-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="b70a6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b70a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b70a6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b70a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b70a6-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b70a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b70a6-107">Intune 的基于角色的访问控制决定哪些人可以对 Intune 对象执行操作并可更改托管应用程序、用户和设备。</span><span class="sxs-lookup"><span data-stu-id="b70a6-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="b70a6-108">以下 Graph 资源可用于管理 Intune 中基于角色的访问控制：</span><span class="sxs-lookup"><span data-stu-id="b70a6-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="b70a6-109">设备和应用管理分配的角色详情</span><span class="sxs-lookup"><span data-stu-id="b70a6-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="b70a6-110">设备和应用管理角色分配</span><span class="sxs-lookup"><span data-stu-id="b70a6-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="b70a6-111">设备和应用管理角色定义</span><span class="sxs-lookup"><span data-stu-id="b70a6-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="b70a6-112">资源操作</span><span class="sxs-lookup"><span data-stu-id="b70a6-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="b70a6-113">资源操作</span><span class="sxs-lookup"><span data-stu-id="b70a6-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="b70a6-114">角色分配</span><span class="sxs-lookup"><span data-stu-id="b70a6-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="b70a6-115">角色分配范围类型</span><span class="sxs-lookup"><span data-stu-id="b70a6-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="b70a6-116">角色定义</span><span class="sxs-lookup"><span data-stu-id="b70a6-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="b70a6-117">角色权限</span><span class="sxs-lookup"><span data-stu-id="b70a6-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="b70a6-118">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="b70a6-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="b70a6-119">角色作用域标记自动分配</span><span class="sxs-lookup"><span data-stu-id="b70a6-119">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)
