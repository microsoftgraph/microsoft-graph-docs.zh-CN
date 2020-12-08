---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f2b4fbc4b4a496905f8199b065ecd94e849365e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581195"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="76a18-103">defaultUserRolePermissions 资源类型</span><span class="sxs-lookup"><span data-stu-id="76a18-103">defaultUserRolePermissions resource type</span></span>

<span data-ttu-id="76a18-104">包含 Azure Active Directory (AD) 中的默认用户角色的一些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="76a18-104">Contains certain customizable permissions of default user role in Azure Active Directory (AD).</span></span>

## <a name="properties"></a><span data-ttu-id="76a18-105">属性</span><span class="sxs-lookup"><span data-stu-id="76a18-105">Properties</span></span>

| <span data-ttu-id="76a18-106">属性</span><span class="sxs-lookup"><span data-stu-id="76a18-106">Property</span></span> | <span data-ttu-id="76a18-107">类型</span><span class="sxs-lookup"><span data-stu-id="76a18-107">Type</span></span> | <span data-ttu-id="76a18-108">Description</span><span class="sxs-lookup"><span data-stu-id="76a18-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="76a18-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="76a18-109">allowedToCreateApps</span></span> | <span data-ttu-id="76a18-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="76a18-110">Boolean</span></span> | <span data-ttu-id="76a18-111">指示默认用户角色是否可以创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="76a18-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="76a18-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="76a18-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="76a18-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="76a18-113">Boolean</span></span> | <span data-ttu-id="76a18-114">指示默认用户角色是否可以创建安全组。</span><span class="sxs-lookup"><span data-stu-id="76a18-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="76a18-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="76a18-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="76a18-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="76a18-116">Boolean</span></span> | <span data-ttu-id="76a18-117">指示默认用户角色是否可以读取其他用户。</span><span class="sxs-lookup"><span data-stu-id="76a18-117">Indicates whether the default user role can read other users.</span></span> |
|<span data-ttu-id="76a18-118">permissionGrantPoliciesAssigned</span><span class="sxs-lookup"><span data-stu-id="76a18-118">permissionGrantPoliciesAssigned</span></span>|<span data-ttu-id="76a18-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="76a18-119">String collection</span></span>|<span data-ttu-id="76a18-120">指示是否允许用户同意应用程序，如果是，授予同意的权限以及 (permissionGrantPolicy 的应用程序同意策略) 管理用户授予同意的权限。</span><span class="sxs-lookup"><span data-stu-id="76a18-120">Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.</span></span> <span data-ttu-id="76a18-121">值的格式应为 `managePermissionGrantsForSelf.{id}` ，其中 `{id}` 是内置或自定义 [应用程序许可策略](/azure/active-directory/manage-apps/manage-app-consent-policies)的 **id** 。</span><span class="sxs-lookup"><span data-stu-id="76a18-121">Value should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="76a18-122">空列表指示用户同意应用程序已被禁用。</span><span class="sxs-lookup"><span data-stu-id="76a18-122">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="76a18-123">关系</span><span class="sxs-lookup"><span data-stu-id="76a18-123">Relationships</span></span>

<span data-ttu-id="76a18-124">无。</span><span class="sxs-lookup"><span data-stu-id="76a18-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76a18-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76a18-125">JSON representation</span></span>

<span data-ttu-id="76a18-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76a18-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true,
  "permissionGrantPoliciesAssigned": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
