---
title: Microsoft Intune 中的基于角色的访问控制
description: 列出用于定义和管理租户组织的基于角色的访问控制 (RBAC) 的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 7bb65853c04ebe7595dfd302e9836b51fcb7cfac
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940020"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="e84eb-103">Microsoft Intune 中的基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="e84eb-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="e84eb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e84eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e84eb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e84eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e84eb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e84eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="e84eb-107">Intune 的基于角色的访问控制决定哪些人可以对 Intune 对象执行操作并可更改托管应用程序、用户和设备。</span><span class="sxs-lookup"><span data-stu-id="e84eb-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="e84eb-108">以下 Graph 资源可用于管理 Intune 中基于角色的访问控制：</span><span class="sxs-lookup"><span data-stu-id="e84eb-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="e84eb-109">设备和应用管理分配的角色详情</span><span class="sxs-lookup"><span data-stu-id="e84eb-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="e84eb-110">设备和应用管理角色分配</span><span class="sxs-lookup"><span data-stu-id="e84eb-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="e84eb-111">设备和应用管理角色定义</span><span class="sxs-lookup"><span data-stu-id="e84eb-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="e84eb-112">资源操作</span><span class="sxs-lookup"><span data-stu-id="e84eb-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="e84eb-113">资源操作</span><span class="sxs-lookup"><span data-stu-id="e84eb-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="e84eb-114">角色分配</span><span class="sxs-lookup"><span data-stu-id="e84eb-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="e84eb-115">角色分配范围类型</span><span class="sxs-lookup"><span data-stu-id="e84eb-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="e84eb-116">角色定义</span><span class="sxs-lookup"><span data-stu-id="e84eb-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="e84eb-117">角色权限</span><span class="sxs-lookup"><span data-stu-id="e84eb-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="e84eb-118">角色范围标记</span><span class="sxs-lookup"><span data-stu-id="e84eb-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
