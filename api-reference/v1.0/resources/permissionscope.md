---
title: permissionScope 资源类型
description: 表示 OAuth 2.0 委派的权限范围。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: be8d9a7d08334bd716cfcbf565225add790b65e3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939367"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="1d051-103">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d051-103">permissionScope resource type</span></span>

<span data-ttu-id="1d051-104">表示 OAuth 2.0 委派的权限范围。</span><span class="sxs-lookup"><span data-stu-id="1d051-104">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="1d051-105">调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过[application](application.md)对象上的**requiredResourceAccess**集合）。</span><span class="sxs-lookup"><span data-stu-id="1d051-105">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="1d051-106">**Oauth2Permissions**属性</span><span class="sxs-lookup"><span data-stu-id="1d051-106">The **oauth2Permissions** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="1d051-107">[应用程序](application.md)实体是**permissionScope**的集合。</span><span class="sxs-lookup"><span data-stu-id="1d051-107">of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="1d051-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d051-108">Properties</span></span>

| <span data-ttu-id="1d051-109">属性</span><span class="sxs-lookup"><span data-stu-id="1d051-109">Property</span></span> | <span data-ttu-id="1d051-110">类型</span><span class="sxs-lookup"><span data-stu-id="1d051-110">Type</span></span> | <span data-ttu-id="1d051-111">描述</span><span class="sxs-lookup"><span data-stu-id="1d051-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1d051-112">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="1d051-112">adminConsentDescription</span></span>|<span data-ttu-id="1d051-113">String</span><span class="sxs-lookup"><span data-stu-id="1d051-113">String</span></span>| <span data-ttu-id="1d051-114">管理员同意和应用工作分配体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="1d051-114">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="1d051-115">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="1d051-115">adminConsentDisplayName</span></span>|<span data-ttu-id="1d051-116">String</span><span class="sxs-lookup"><span data-stu-id="1d051-116">String</span></span>| <span data-ttu-id="1d051-117">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1d051-117">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="1d051-118">id</span><span class="sxs-lookup"><span data-stu-id="1d051-118">id</span></span>|<span data-ttu-id="1d051-119">Guid</span><span class="sxs-lookup"><span data-stu-id="1d051-119">Guid</span></span>| <span data-ttu-id="1d051-120">Oauth2Permissions 集合中的唯一作用域权限标识符。</span><span class="sxs-lookup"><span data-stu-id="1d051-120">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="1d051-121">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1d051-121">isEnabled</span></span>|<span data-ttu-id="1d051-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d051-122">Boolean</span></span>| <span data-ttu-id="1d051-123">在创建或更新权限时，此属性必须设置为**true** （默认值）。</span><span class="sxs-lookup"><span data-stu-id="1d051-123">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="1d051-124">若要删除权限，必须首先将此属性设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="1d051-124">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="1d051-125">此时，在后续调用中，可能会删除该权限。</span><span class="sxs-lookup"><span data-stu-id="1d051-125">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="1d051-126">格式</span><span class="sxs-lookup"><span data-stu-id="1d051-126">origin</span></span>|<span data-ttu-id="1d051-127">String</span><span class="sxs-lookup"><span data-stu-id="1d051-127">String</span></span>| <span data-ttu-id="1d051-128">供内部使用。</span><span class="sxs-lookup"><span data-stu-id="1d051-128">For internal use.</span></span> |
|<span data-ttu-id="1d051-129">type</span><span class="sxs-lookup"><span data-stu-id="1d051-129">type</span></span>|<span data-ttu-id="1d051-130">String</span><span class="sxs-lookup"><span data-stu-id="1d051-130">String</span></span>| <span data-ttu-id="1d051-131">指定此范围权限是否可由最终用户许可，或者是否为公司管理员必须同意的租户范围内的权限。</span><span class="sxs-lookup"><span data-stu-id="1d051-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="1d051-132">可能的值为*User*或*Admin*。</span><span class="sxs-lookup"><span data-stu-id="1d051-132">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="1d051-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="1d051-133">userConsentDescription</span></span>|<span data-ttu-id="1d051-134">String</span><span class="sxs-lookup"><span data-stu-id="1d051-134">String</span></span>| <span data-ttu-id="1d051-135">最终用户同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="1d051-135">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="1d051-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="1d051-136">userConsentDisplayName</span></span>|<span data-ttu-id="1d051-137">String</span><span class="sxs-lookup"><span data-stu-id="1d051-137">String</span></span>| <span data-ttu-id="1d051-138">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1d051-138">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="1d051-139">value</span><span class="sxs-lookup"><span data-stu-id="1d051-139">value</span></span>|<span data-ttu-id="1d051-140">String</span><span class="sxs-lookup"><span data-stu-id="1d051-140">String</span></span>| <span data-ttu-id="1d051-141">在 OAuth 2.0 访问令牌中，资源应用程序应期望的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="1d051-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1d051-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d051-142">JSON representation</span></span>
<span data-ttu-id="1d051-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d051-143">Here is a JSON representation of the resource.</span></span>

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
