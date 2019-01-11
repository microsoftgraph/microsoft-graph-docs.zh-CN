---
title: Microsoft Intune 中的基于角色的访问控制
description: 'Intune 的基于角色的访问控制决定哪些人可以对 Intune 对象执行操作并可更改托管应用程序、用户和设备。   '
localization_priority: Normal
ms.openlocfilehash: 7772ad42d96f6c8907f813e8e62cfb4429fe2cc2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804884"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="b2134-103">Microsoft Intune 中的基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="b2134-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="b2134-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b2134-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2134-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b2134-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2134-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b2134-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b2134-107">Intune 的基于角色的访问控制决定哪些人可以对 Intune 对象执行操作并可更改托管应用程序、用户和设备。</span><span class="sxs-lookup"><span data-stu-id="b2134-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="b2134-108">以下 Graph 资源可用于管理 Intune 中基于角色的访问控制：</span><span class="sxs-lookup"><span data-stu-id="b2134-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="b2134-109">分配角色 id 的设备和应用程序管理</span><span class="sxs-lookup"><span data-stu-id="b2134-109">Device and app management assigned role ids</span></span>](intune-rbac-deviceandappmanagementassignedroleids.md)
- [<span data-ttu-id="b2134-110">设备和应用管理角色分配</span><span class="sxs-lookup"><span data-stu-id="b2134-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="b2134-111">设备和应用管理角色定义</span><span class="sxs-lookup"><span data-stu-id="b2134-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="b2134-112">资源操作</span><span class="sxs-lookup"><span data-stu-id="b2134-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="b2134-113">资源操作</span><span class="sxs-lookup"><span data-stu-id="b2134-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="b2134-114">角色分配</span><span class="sxs-lookup"><span data-stu-id="b2134-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="b2134-115">角色分配范围类型</span><span class="sxs-lookup"><span data-stu-id="b2134-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="b2134-116">角色定义</span><span class="sxs-lookup"><span data-stu-id="b2134-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="b2134-117">角色权限</span><span class="sxs-lookup"><span data-stu-id="b2134-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="b2134-118">角色作用域标记</span><span class="sxs-lookup"><span data-stu-id="b2134-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
