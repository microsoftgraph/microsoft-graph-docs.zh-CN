---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e89f175a62615efe172646613897222a9ae75fa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137555"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="c72ab-103">defaultUserRolePermissions 资源类型</span><span class="sxs-lookup"><span data-stu-id="c72ab-103">defaultUserRolePermissions resource type</span></span>

<span data-ttu-id="c72ab-104">包含 Azure Active Directory 中默认用户角色的某些可自定义权限 (AD) 。</span><span class="sxs-lookup"><span data-stu-id="c72ab-104">Contains certain customizable permissions of default user role in Azure Active Directory (AD).</span></span>

## <a name="properties"></a><span data-ttu-id="c72ab-105">属性</span><span class="sxs-lookup"><span data-stu-id="c72ab-105">Properties</span></span>

| <span data-ttu-id="c72ab-106">属性</span><span class="sxs-lookup"><span data-stu-id="c72ab-106">Property</span></span> | <span data-ttu-id="c72ab-107">类型</span><span class="sxs-lookup"><span data-stu-id="c72ab-107">Type</span></span> | <span data-ttu-id="c72ab-108">说明</span><span class="sxs-lookup"><span data-stu-id="c72ab-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="c72ab-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="c72ab-109">allowedToCreateApps</span></span> | <span data-ttu-id="c72ab-110">布尔</span><span class="sxs-lookup"><span data-stu-id="c72ab-110">Boolean</span></span> | <span data-ttu-id="c72ab-111">指示默认用户角色是否可以创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="c72ab-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="c72ab-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="c72ab-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="c72ab-113">布尔</span><span class="sxs-lookup"><span data-stu-id="c72ab-113">Boolean</span></span> | <span data-ttu-id="c72ab-114">指示默认用户角色是否可以创建安全组。</span><span class="sxs-lookup"><span data-stu-id="c72ab-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="c72ab-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="c72ab-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="c72ab-116">布尔</span><span class="sxs-lookup"><span data-stu-id="c72ab-116">Boolean</span></span> | <span data-ttu-id="c72ab-117">指示默认用户角色是否可以读取其他用户。</span><span class="sxs-lookup"><span data-stu-id="c72ab-117">Indicates whether the default user role can read other users.</span></span> |
|<span data-ttu-id="c72ab-118">permissionGrantPoliciesAssigned</span><span class="sxs-lookup"><span data-stu-id="c72ab-118">permissionGrantPoliciesAssigned</span></span>|<span data-ttu-id="c72ab-119">String collection</span><span class="sxs-lookup"><span data-stu-id="c72ab-119">String collection</span></span>|<span data-ttu-id="c72ab-120">指示是否允许用户同意应用，如果允许，授予许可的权限以及哪个应用许可策略 (permissionGrantPolicy) 管理用户授予同意的权限。</span><span class="sxs-lookup"><span data-stu-id="c72ab-120">Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.</span></span> <span data-ttu-id="c72ab-121">值的格式应为，其中是内置或自定义应用同意 `managePermissionGrantsForSelf.{id}` `{id}` [策略的 ID。](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="c72ab-121">Value should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="c72ab-122">空列表指示用户已禁用对应用的同意。</span><span class="sxs-lookup"><span data-stu-id="c72ab-122">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c72ab-123">关系</span><span class="sxs-lookup"><span data-stu-id="c72ab-123">Relationships</span></span>

<span data-ttu-id="c72ab-124">无。</span><span class="sxs-lookup"><span data-stu-id="c72ab-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c72ab-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c72ab-125">JSON representation</span></span>

<span data-ttu-id="c72ab-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c72ab-126">The following is a JSON representation of the resource.</span></span>

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
