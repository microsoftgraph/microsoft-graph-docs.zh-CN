---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6fc799fec39eaa209ac8e74b02743cf84e76a51a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316476"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="f96d1-103">unifiedRolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="f96d1-103">unifiedRolePermission resource type</span></span>

<span data-ttu-id="f96d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f96d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f96d1-105">表示允许的资源操作的集合以及使操作生效所必须满足的条件。</span><span class="sxs-lookup"><span data-stu-id="f96d1-105">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="f96d1-106">资源操作是可在资源上执行的任务。</span><span class="sxs-lookup"><span data-stu-id="f96d1-106">Resource actions are tasks that can be performed on a resource.</span></span> <span data-ttu-id="f96d1-107">例如，应用程序资源支持创建、更新、删除和重置密码资源操作。</span><span class="sxs-lookup"><span data-stu-id="f96d1-107">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="f96d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="f96d1-108">Properties</span></span>

| <span data-ttu-id="f96d1-109">属性</span><span class="sxs-lookup"><span data-stu-id="f96d1-109">Property</span></span>     | <span data-ttu-id="f96d1-110">类型</span><span class="sxs-lookup"><span data-stu-id="f96d1-110">Type</span></span>        | <span data-ttu-id="f96d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="f96d1-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f96d1-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="f96d1-112">allowedResourceActions</span></span>|<span data-ttu-id="f96d1-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="f96d1-113">String collection</span></span>| <span data-ttu-id="f96d1-114">可在资源上执行的任务集。</span><span class="sxs-lookup"><span data-stu-id="f96d1-114">Set of tasks that can be performed on a resource.</span></span> |
|<span data-ttu-id="f96d1-115">condition</span><span class="sxs-lookup"><span data-stu-id="f96d1-115">condition</span></span>|<span data-ttu-id="f96d1-116">字符串</span><span class="sxs-lookup"><span data-stu-id="f96d1-116">String</span></span>| <span data-ttu-id="f96d1-117">权限生效所必须满足的可选约束。</span><span class="sxs-lookup"><span data-stu-id="f96d1-117">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="f96d1-118">allowedResourceActions 属性</span><span class="sxs-lookup"><span data-stu-id="f96d1-118">allowedResourceActions property</span></span>

<span data-ttu-id="f96d1-119">下面是资源操作架构：</span><span class="sxs-lookup"><span data-stu-id="f96d1-119">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="f96d1-120">例如：`microsoft.directory/applications/credentials/update`。</span><span class="sxs-lookup"><span data-stu-id="f96d1-120">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="f96d1-121">命名空间 - 公开任务的服务。</span><span class="sxs-lookup"><span data-stu-id="f96d1-121">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="f96d1-122">例如，所有任务Azure Active Directory命名空间 microsoft.directory。</span><span class="sxs-lookup"><span data-stu-id="f96d1-122">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="f96d1-123">Entity - Microsoft 服务公开的逻辑功能或Graph。</span><span class="sxs-lookup"><span data-stu-id="f96d1-123">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="f96d1-124">例如，应用程序、服务主体或组。</span><span class="sxs-lookup"><span data-stu-id="f96d1-124">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="f96d1-125">PropertySet - 要授予其访问权限的实体的特定属性或方面。</span><span class="sxs-lookup"><span data-stu-id="f96d1-125">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="f96d1-126">例如，授予在 Azure AD 中读取应用程序对象上的回复 URL、注销 URL 和隐式流 `microsoft.directory/applications/authentication/read` 属性的能力。 </span><span class="sxs-lookup"><span data-stu-id="f96d1-126">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="f96d1-127">以下是常见属性集的保留名称：</span><span class="sxs-lookup"><span data-stu-id="f96d1-127">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="f96d1-128">allProperties - 指定实体的所有属性，包括特权属性。</span><span class="sxs-lookup"><span data-stu-id="f96d1-128">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="f96d1-129">示例包括 `microsoft.directory/applications/allProperties/read` `microsoft.directory/applications/allProperties/update` 和 。</span><span class="sxs-lookup"><span data-stu-id="f96d1-129">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="f96d1-130">basic - 指定常用读取属性，但不包括特权属性。</span><span class="sxs-lookup"><span data-stu-id="f96d1-130">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="f96d1-131">例如， `microsoft.directory/applications/basic/update` 包括更新标准属性（如 显示名称）。</span><span class="sxs-lookup"><span data-stu-id="f96d1-131">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="f96d1-132">standard - 指定常用更新属性，但不包括特权属性。</span><span class="sxs-lookup"><span data-stu-id="f96d1-132">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="f96d1-133">例如，`microsoft.directory/applications/standard/read`。</span><span class="sxs-lookup"><span data-stu-id="f96d1-133">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="f96d1-134">操作 - 要授予的操作。</span><span class="sxs-lookup"><span data-stu-id="f96d1-134">Actions - The operations being granted.</span></span> <span data-ttu-id="f96d1-135">在大多数情况下，权限应表示为 CRUD 或 allTasks。</span><span class="sxs-lookup"><span data-stu-id="f96d1-135">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="f96d1-136">操作包括：</span><span class="sxs-lookup"><span data-stu-id="f96d1-136">Actions include:</span></span>
  - <span data-ttu-id="f96d1-137">Create - 创建实体的新实例的能力。</span><span class="sxs-lookup"><span data-stu-id="f96d1-137">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="f96d1-138">读取 - 读取给定属性集 (包括 allProperties) 。</span><span class="sxs-lookup"><span data-stu-id="f96d1-138">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="f96d1-139">Update - 更新给定属性集 (包括 allProperties) 。</span><span class="sxs-lookup"><span data-stu-id="f96d1-139">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="f96d1-140">Delete - 删除给定实体的能力。</span><span class="sxs-lookup"><span data-stu-id="f96d1-140">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="f96d1-141">AllTasks - 表示创建、 (、更新和删除文件的所有 CRUD) 。</span><span class="sxs-lookup"><span data-stu-id="f96d1-141">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="f96d1-142">condition 属性</span><span class="sxs-lookup"><span data-stu-id="f96d1-142">condition property</span></span>
<span data-ttu-id="f96d1-143">条件定义必须满足的约束。</span><span class="sxs-lookup"><span data-stu-id="f96d1-143">Conditions define constraints that must be met.</span></span> <span data-ttu-id="f96d1-144">例如，要求主体是目标"所有者"的要求。</span><span class="sxs-lookup"><span data-stu-id="f96d1-144">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="f96d1-145">以下是受支持的条件：</span><span class="sxs-lookup"><span data-stu-id="f96d1-145">The following are the supported conditions:</span></span>

- <span data-ttu-id="f96d1-146">自我："$ResourceIsSelf"</span><span class="sxs-lookup"><span data-stu-id="f96d1-146">Self: "$ResourceIsSelf"</span></span>
- <span data-ttu-id="f96d1-147">所有者："$SubjectIsOwner"</span><span class="sxs-lookup"><span data-stu-id="f96d1-147">Owner: "$SubjectIsOwner"</span></span>

<span data-ttu-id="f96d1-148">下面是具有条件的角色权限的示例。</span><span class="sxs-lookup"><span data-stu-id="f96d1-148">The following is an example of a role permission with a condition.</span></span>

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "$SubjectIsOwner"
        }
    ]

```

## <a name="json-representation"></a><span data-ttu-id="f96d1-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f96d1-149">JSON representation</span></span>

<span data-ttu-id="f96d1-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f96d1-150">The following is a JSON representation of the resource.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="f96d1-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f96d1-151">See also</span></span>

- <span data-ttu-id="f96d1-152">[管理员角色权限Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - 有关内置目录角色的权限的信息。</span><span class="sxs-lookup"><span data-stu-id="f96d1-152">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="f96d1-153">[应用程序注册子类型和](/azure/active-directory/users-groups-roles/roles-custom-available-permissions)Azure Active Directory - 有关可用于自定义目录角色的权限的信息。</span><span class="sxs-lookup"><span data-stu-id="f96d1-153">[Application registration subtypes and permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
