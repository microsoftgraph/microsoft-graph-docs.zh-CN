---
title: permissionScope 资源类型
description: 表示 OAuth 2.0 委派的权限范围。 调用资源应用程序时, 客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围 (通过 Application 对象上的**requiredResourceAccess**集合)。 ServicePrincipal 实体和 Application 实体的**oauth2Permissions**属性是**OAuth2Permission**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 59770460b8fbc3c0a8946eeed94adfbe027f20cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966163"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="a8a9d-105">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8a9d-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8a9d-106">表示 OAuth 2.0 委派的权限范围。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="a8a9d-107">调用资源应用程序时, 客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围 (通过[application](application.md)对象上的**requiredResourceAccess**集合)。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="a8a9d-108">[ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**oauth2Permissions**属性是**OAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-108">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="a8a9d-109">属性</span><span class="sxs-lookup"><span data-stu-id="a8a9d-109">Properties</span></span>

| <span data-ttu-id="a8a9d-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8a9d-110">Property</span></span> | <span data-ttu-id="a8a9d-111">类型</span><span class="sxs-lookup"><span data-stu-id="a8a9d-111">Type</span></span> | <span data-ttu-id="a8a9d-112">说明</span><span class="sxs-lookup"><span data-stu-id="a8a9d-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8a9d-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="a8a9d-113">adminConsentDescription</span></span>|<span data-ttu-id="a8a9d-114">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-114">String</span></span>| <span data-ttu-id="a8a9d-115">管理员同意和应用工作分配体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="a8a9d-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="a8a9d-116">adminConsentDisplayName</span></span>|<span data-ttu-id="a8a9d-117">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-117">String</span></span>| <span data-ttu-id="a8a9d-118">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="a8a9d-119">id</span><span class="sxs-lookup"><span data-stu-id="a8a9d-119">id</span></span>|<span data-ttu-id="a8a9d-120">Guid</span><span class="sxs-lookup"><span data-stu-id="a8a9d-120">Guid</span></span>| <span data-ttu-id="a8a9d-121">Oauth2Permissions 集合中的唯一作用域权限标识符。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="a8a9d-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a8a9d-122">isEnabled</span></span>|<span data-ttu-id="a8a9d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8a9d-123">Boolean</span></span>| <span data-ttu-id="a8a9d-124">在创建或更新权限时, 此属性必须设置为**true** (默认值)。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="a8a9d-125">若要删除权限, 必须首先将此属性设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="a8a9d-126">此时, 在后续调用中, 可能会删除该权限。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="a8a9d-127">格式</span><span class="sxs-lookup"><span data-stu-id="a8a9d-127">origin</span></span>|<span data-ttu-id="a8a9d-128">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-128">String</span></span>| <span data-ttu-id="a8a9d-129">供内部使用。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-129">For internal use.</span></span> |
|<span data-ttu-id="a8a9d-130">type</span><span class="sxs-lookup"><span data-stu-id="a8a9d-130">type</span></span>|<span data-ttu-id="a8a9d-131">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-131">String</span></span>| <span data-ttu-id="a8a9d-132">指定此范围权限是否可由最终用户许可, 或者是否为公司管理员必须同意的租户范围内的权限。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="a8a9d-133">可能的值为*User*或*Admin*。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="a8a9d-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="a8a9d-134">userConsentDescription</span></span>|<span data-ttu-id="a8a9d-135">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-135">String</span></span>| <span data-ttu-id="a8a9d-136">最终用户同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="a8a9d-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="a8a9d-137">userConsentDisplayName</span></span>|<span data-ttu-id="a8a9d-138">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-138">String</span></span>| <span data-ttu-id="a8a9d-139">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="a8a9d-140">value</span><span class="sxs-lookup"><span data-stu-id="a8a9d-140">value</span></span>|<span data-ttu-id="a8a9d-141">String</span><span class="sxs-lookup"><span data-stu-id="a8a9d-141">String</span></span>| <span data-ttu-id="a8a9d-142">在 OAuth 2.0 访问令牌中, 资源应用程序应期望的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8a9d-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8a9d-143">JSON representation</span></span>
<span data-ttu-id="a8a9d-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8a9d-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
