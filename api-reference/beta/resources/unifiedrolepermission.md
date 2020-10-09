---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa327935c4e3b45c28a0f7ae01ababeffe37d61d
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405223"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="52a32-103">unifiedRolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="52a32-103">unifiedRolePermission resource type</span></span>

<span data-ttu-id="52a32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52a32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a32-105">表示允许的资源操作的集合，以及操作有效时必须满足的条件。</span><span class="sxs-lookup"><span data-stu-id="52a32-105">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="52a32-106">资源操作是可在资源上 perfomed 的任务。</span><span class="sxs-lookup"><span data-stu-id="52a32-106">Resource actions are tasks that can be perfomed on a resource.</span></span> <span data-ttu-id="52a32-107">例如，应用程序资源支持创建、更新、删除和重置密码资源操作。</span><span class="sxs-lookup"><span data-stu-id="52a32-107">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="52a32-108">属性</span><span class="sxs-lookup"><span data-stu-id="52a32-108">Properties</span></span>

| <span data-ttu-id="52a32-109">属性</span><span class="sxs-lookup"><span data-stu-id="52a32-109">Property</span></span>     | <span data-ttu-id="52a32-110">类型</span><span class="sxs-lookup"><span data-stu-id="52a32-110">Type</span></span>        | <span data-ttu-id="52a32-111">说明</span><span class="sxs-lookup"><span data-stu-id="52a32-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52a32-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="52a32-112">allowedResourceActions</span></span>|<span data-ttu-id="52a32-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="52a32-113">String collection</span></span>| <span data-ttu-id="52a32-114">可在资源上 perfomed 的一组任务。</span><span class="sxs-lookup"><span data-stu-id="52a32-114">Set of tasks that can be perfomed on a resource.</span></span> |
|<span data-ttu-id="52a32-115">表达式</span><span class="sxs-lookup"><span data-stu-id="52a32-115">condition</span></span>|<span data-ttu-id="52a32-116">字符串</span><span class="sxs-lookup"><span data-stu-id="52a32-116">String</span></span>| <span data-ttu-id="52a32-117">要使权限生效必须满足的可选约束。</span><span class="sxs-lookup"><span data-stu-id="52a32-117">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="52a32-118">allowedResourceActions 属性</span><span class="sxs-lookup"><span data-stu-id="52a32-118">allowedResourceActions property</span></span>

<span data-ttu-id="52a32-119">以下是资源操作的架构：</span><span class="sxs-lookup"><span data-stu-id="52a32-119">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="52a32-120">例如：`microsoft.directory/applications/credentials/update`。</span><span class="sxs-lookup"><span data-stu-id="52a32-120">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="52a32-121">命名空间-公开任务的服务。</span><span class="sxs-lookup"><span data-stu-id="52a32-121">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="52a32-122">例如，Azure Active Directory 中的所有任务都使用命名空间 "microsoft."。</span><span class="sxs-lookup"><span data-stu-id="52a32-122">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="52a32-123">Entity-Microsoft Graph 中的服务公开的逻辑功能或组件。</span><span class="sxs-lookup"><span data-stu-id="52a32-123">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="52a32-124">例如，应用程序、服务主体或组。</span><span class="sxs-lookup"><span data-stu-id="52a32-124">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="52a32-125">PropertySet-要为其授予访问权限的实体的特定属性或方面。</span><span class="sxs-lookup"><span data-stu-id="52a32-125">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="52a32-126">例如， `microsoft.directory/applications/authentication/read` 向 AZURE AD 中的 **application** 对象授予读取回复 URL、注销 url 和隐式流属性的功能。</span><span class="sxs-lookup"><span data-stu-id="52a32-126">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="52a32-127">以下是常用属性集的保留名称：</span><span class="sxs-lookup"><span data-stu-id="52a32-127">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="52a32-128">allProperties-指定实体的所有属性，包括特权属性。</span><span class="sxs-lookup"><span data-stu-id="52a32-128">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="52a32-129">示例包括 `microsoft.directory/applications/allProperties/read` 和 `microsoft.directory/applications/allProperties/update` 。</span><span class="sxs-lookup"><span data-stu-id="52a32-129">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="52a32-130">basic-指定常见的读取属性，但不包括特权。</span><span class="sxs-lookup"><span data-stu-id="52a32-130">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="52a32-131">例如， `microsoft.directory/applications/basic/update` 包括更新显示名称等标准属性的功能。</span><span class="sxs-lookup"><span data-stu-id="52a32-131">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="52a32-132">standard-指定通用更新属性，但不包括特权文件。</span><span class="sxs-lookup"><span data-stu-id="52a32-132">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="52a32-133">例如，`microsoft.directory/applications/standard/read`。</span><span class="sxs-lookup"><span data-stu-id="52a32-133">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="52a32-134">操作-要授予的操作。</span><span class="sxs-lookup"><span data-stu-id="52a32-134">Actions - The operations being granted.</span></span> <span data-ttu-id="52a32-135">在大多数情况下，应根据 CRUD 或 allTasks 表示权限。</span><span class="sxs-lookup"><span data-stu-id="52a32-135">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="52a32-136">操作包括：</span><span class="sxs-lookup"><span data-stu-id="52a32-136">Actions include:</span></span>
  - <span data-ttu-id="52a32-137">创建-创建实体的新实例的功能。</span><span class="sxs-lookup"><span data-stu-id="52a32-137">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="52a32-138">Read-读取给定属性集 (包括 allProperties) 的功能。</span><span class="sxs-lookup"><span data-stu-id="52a32-138">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="52a32-139">Update-更新给定属性集 (包括 allProperties) 的功能。</span><span class="sxs-lookup"><span data-stu-id="52a32-139">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="52a32-140">删除-删除给定实体的功能。</span><span class="sxs-lookup"><span data-stu-id="52a32-140">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="52a32-141">AllTasks-表示 (创建、读取、更新和删除) 的所有 CRUD 操作。</span><span class="sxs-lookup"><span data-stu-id="52a32-141">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="52a32-142">condition 属性</span><span class="sxs-lookup"><span data-stu-id="52a32-142">condition property</span></span>
<span data-ttu-id="52a32-143">条件定义必须满足的约束。</span><span class="sxs-lookup"><span data-stu-id="52a32-143">Conditions define constraints that must be met.</span></span> <span data-ttu-id="52a32-144">例如，要求主体是目标的 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="52a32-144">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="52a32-145">以下是受支持的条件：</span><span class="sxs-lookup"><span data-stu-id="52a32-145">The following are the supported conditions:</span></span>

- <span data-ttu-id="52a32-146">Self： "@Subject = = @Resource objectId"</span><span class="sxs-lookup"><span data-stu-id="52a32-146">Self: "@Subject.objectId == @Resource.objectId"</span></span>
- <span data-ttu-id="52a32-147">Owner： "@Subject Any_of @Resource 所有者"</span><span class="sxs-lookup"><span data-stu-id="52a32-147">Owner: "@Subject.objectId Any_of @Resource.owners"</span></span>

<span data-ttu-id="52a32-148">下面是具有条件的角色权限的一个示例。</span><span class="sxs-lookup"><span data-stu-id="52a32-148">The following is an example of a role permission with a condition.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="52a32-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52a32-149">JSON representation</span></span>

<span data-ttu-id="52a32-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52a32-150">The following is a JSON representation of the resource.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="52a32-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="52a32-151">See also</span></span>

- <span data-ttu-id="52a32-152">[Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) -用于有关内置目录角色的权限的信息。</span><span class="sxs-lookup"><span data-stu-id="52a32-152">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="52a32-153">[Azure Active Directory 中的应用程序注册子类型和权限](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -有关可用于自定义目录角色的权限的信息。</span><span class="sxs-lookup"><span data-stu-id="52a32-153">[Application registration subtypes and permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->