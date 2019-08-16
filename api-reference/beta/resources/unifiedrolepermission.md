---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d15e2709c429be3c6400b59db5174093892d3009
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437858"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="f7c8b-103">unifiedRolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7c8b-103">unifiedRolePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c8b-104">表示允许的资源操作的集合, 以及操作有效时必须满足的条件。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-104">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="f7c8b-105">资源操作是可在资源上 perfomed 的任务。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-105">Resource actions are tasks that can be perfomed on a resource.</span></span> <span data-ttu-id="f7c8b-106">例如, 应用程序资源支持创建、更新、删除和重置密码资源操作。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-106">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="f7c8b-107">属性</span><span class="sxs-lookup"><span data-stu-id="f7c8b-107">Properties</span></span>

| <span data-ttu-id="f7c8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7c8b-108">Property</span></span>     | <span data-ttu-id="f7c8b-109">类型</span><span class="sxs-lookup"><span data-stu-id="f7c8b-109">Type</span></span>        | <span data-ttu-id="f7c8b-110">说明</span><span class="sxs-lookup"><span data-stu-id="f7c8b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7c8b-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="f7c8b-111">allowedResourceActions</span></span>|<span data-ttu-id="f7c8b-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="f7c8b-112">String collection</span></span>| <span data-ttu-id="f7c8b-113">可在资源上 perfomed 的一组任务。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-113">Set of tasks that can be perfomed on a resource.</span></span> |
|<span data-ttu-id="f7c8b-114">表达式</span><span class="sxs-lookup"><span data-stu-id="f7c8b-114">condition</span></span>|<span data-ttu-id="f7c8b-115">String</span><span class="sxs-lookup"><span data-stu-id="f7c8b-115">String</span></span>| <span data-ttu-id="f7c8b-116">要使权限生效必须满足的可选约束。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-116">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="f7c8b-117">allowedResourceActions 属性</span><span class="sxs-lookup"><span data-stu-id="f7c8b-117">allowedResourceActions property</span></span>

<span data-ttu-id="f7c8b-118">以下是资源操作的架构:</span><span class="sxs-lookup"><span data-stu-id="f7c8b-118">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="f7c8b-119">例如：`microsoft.directory/applications/credentials/update`。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-119">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="f7c8b-120">命名空间-公开任务的服务。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-120">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="f7c8b-121">例如, Azure Active Directory 中的所有任务都使用命名空间 "microsoft."。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-121">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="f7c8b-122">Entity-Microsoft Graph 中的服务公开的逻辑功能或组件。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-122">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="f7c8b-123">例如, 应用程序、服务主体或组。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-123">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="f7c8b-124">PropertySet-要为其授予访问权限的实体的特定属性或方面。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-124">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="f7c8b-125">例如, `microsoft.directory/applications/authentication/read`向 Azure AD 中的**application**对象授予读取回复 URL、注销 url 和隐式流属性的功能。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-125">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="f7c8b-126">以下是常用属性集的保留名称:</span><span class="sxs-lookup"><span data-stu-id="f7c8b-126">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="f7c8b-127">allProperties-指定实体的所有属性, 包括特权属性。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-127">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="f7c8b-128">示例包括`microsoft.directory/applications/allProperties/read`和`microsoft.directory/applications/allProperties/update`。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-128">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="f7c8b-129">basic-指定常见的读取属性, 但不包括特权。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-129">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="f7c8b-130">例如, `microsoft.directory/applications/basic/update`包括更新显示名称等标准属性的功能。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-130">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="f7c8b-131">standard-指定通用更新属性, 但不包括特权文件。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-131">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="f7c8b-132">例如，`microsoft.directory/applications/standard/read`。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-132">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="f7c8b-133">操作-要授予的操作。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-133">Actions - The operations being granted.</span></span> <span data-ttu-id="f7c8b-134">在大多数情况下, 应根据 CRUD 或 allTasks 表示权限。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-134">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="f7c8b-135">操作包括:</span><span class="sxs-lookup"><span data-stu-id="f7c8b-135">Actions include:</span></span>
  - <span data-ttu-id="f7c8b-136">创建-创建实体的新实例的功能。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-136">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="f7c8b-137">Read-读取给定属性集的功能 (包括 allProperties)。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-137">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="f7c8b-138">Update-更新给定属性集的能力 (包括 allProperties)。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-138">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="f7c8b-139">删除-删除给定实体的功能。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-139">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="f7c8b-140">AllTasks-表示所有 CRUD 操作 (创建、读取、更新和删除)。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-140">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="f7c8b-141">condition 属性</span><span class="sxs-lookup"><span data-stu-id="f7c8b-141">condition property</span></span>
<span data-ttu-id="f7c8b-142">条件定义必须满足的约束。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-142">Conditions define constraints that must be met.</span></span> <span data-ttu-id="f7c8b-143">例如, 要求主体是目标的 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-143">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="f7c8b-144">以下是受支持的条件:</span><span class="sxs-lookup"><span data-stu-id="f7c8b-144">The following are the supported conditions:</span></span>

- <span data-ttu-id="f7c8b-145">Self: "@Subject = = @Resource objectId"</span><span class="sxs-lookup"><span data-stu-id="f7c8b-145">Self: "@Subject.objectId == @Resource.objectId"</span></span>
- <span data-ttu-id="f7c8b-146">Owner: "@Subject @Resource" Any_of "</span><span class="sxs-lookup"><span data-stu-id="f7c8b-146">Owner: "@Subject.objectId Any_of @Resource.owners"</span></span>

<span data-ttu-id="f7c8b-147">下面是具有条件的角色权限的一个示例。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-147">The following is an example of a role permission with a condition.</span></span>

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "@Subject.objectId Any_of @Resource.owners"
        }
    ]

```

## <a name="json-representation"></a><span data-ttu-id="f7c8b-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7c8b-148">JSON representation</span></span>

<span data-ttu-id="f7c8b-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a><span data-ttu-id="f7c8b-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f7c8b-150">See also</span></span>

- <span data-ttu-id="f7c8b-151">[Azure Active Directory 中的管理员角色权限](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)-用于有关内置目录角色的权限的信息。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-151">[Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="f7c8b-152">[Azure Active Directory 中的应用程序注册子类型和权限](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions)-有关可用于自定义目录角色的权限的信息。</span><span class="sxs-lookup"><span data-stu-id="f7c8b-152">[Application registration subtypes and permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
