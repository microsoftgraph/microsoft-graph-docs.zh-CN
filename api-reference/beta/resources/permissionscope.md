---
title: permissionScope 资源类型
description: 表示 OAuth 2.0 委派的权限范围。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 53e777d3a545ed95c5a6010db7abc965d3b9cad5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939339"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="4a456-103">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a456-103">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a456-104">表示 OAuth 2.0 委派的权限范围。</span><span class="sxs-lookup"><span data-stu-id="4a456-104">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="4a456-105">调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过[application](application.md)对象上的**requiredResourceAccess**集合）。</span><span class="sxs-lookup"><span data-stu-id="4a456-105">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="4a456-106">[ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**oauth2Permissions**属性是**permissionScope**的集合。</span><span class="sxs-lookup"><span data-stu-id="4a456-106">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="4a456-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a456-107">Properties</span></span>

| <span data-ttu-id="4a456-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a456-108">Property</span></span> | <span data-ttu-id="4a456-109">类型</span><span class="sxs-lookup"><span data-stu-id="4a456-109">Type</span></span> | <span data-ttu-id="4a456-110">描述</span><span class="sxs-lookup"><span data-stu-id="4a456-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4a456-111">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="4a456-111">adminConsentDescription</span></span>|<span data-ttu-id="4a456-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4a456-112">String</span></span>| <span data-ttu-id="4a456-113">管理员同意和应用工作分配体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="4a456-113">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="4a456-114">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a456-114">adminConsentDisplayName</span></span>|<span data-ttu-id="4a456-115">字符串</span><span class="sxs-lookup"><span data-stu-id="4a456-115">String</span></span>| <span data-ttu-id="4a456-116">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4a456-116">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="4a456-117">id</span><span class="sxs-lookup"><span data-stu-id="4a456-117">id</span></span>|<span data-ttu-id="4a456-118">Guid</span><span class="sxs-lookup"><span data-stu-id="4a456-118">Guid</span></span>| <span data-ttu-id="4a456-119">Oauth2Permissions 集合中的唯一作用域权限标识符。</span><span class="sxs-lookup"><span data-stu-id="4a456-119">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="4a456-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4a456-120">isEnabled</span></span>|<span data-ttu-id="4a456-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a456-121">Boolean</span></span>| <span data-ttu-id="4a456-122">在创建或更新权限时，此属性必须设置为**true** （默认值）。</span><span class="sxs-lookup"><span data-stu-id="4a456-122">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="4a456-123">若要删除权限，必须首先将此属性设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="4a456-123">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="4a456-124">此时，在后续调用中，可能会删除该权限。</span><span class="sxs-lookup"><span data-stu-id="4a456-124">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="4a456-125">格式</span><span class="sxs-lookup"><span data-stu-id="4a456-125">origin</span></span>|<span data-ttu-id="4a456-126">字符串</span><span class="sxs-lookup"><span data-stu-id="4a456-126">String</span></span>| <span data-ttu-id="4a456-127">供内部使用。</span><span class="sxs-lookup"><span data-stu-id="4a456-127">For internal use.</span></span> |
|<span data-ttu-id="4a456-128">type</span><span class="sxs-lookup"><span data-stu-id="4a456-128">type</span></span>|<span data-ttu-id="4a456-129">字符串</span><span class="sxs-lookup"><span data-stu-id="4a456-129">String</span></span>| <span data-ttu-id="4a456-130">指定此范围权限是否可由最终用户许可，或者是否为公司管理员必须同意的租户范围内的权限。</span><span class="sxs-lookup"><span data-stu-id="4a456-130">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="4a456-131">可能的值为*User*或*Admin*。</span><span class="sxs-lookup"><span data-stu-id="4a456-131">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="4a456-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="4a456-132">userConsentDescription</span></span>|<span data-ttu-id="4a456-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4a456-133">String</span></span>| <span data-ttu-id="4a456-134">最终用户同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="4a456-134">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="4a456-135">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a456-135">userConsentDisplayName</span></span>|<span data-ttu-id="4a456-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4a456-136">String</span></span>| <span data-ttu-id="4a456-137">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4a456-137">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="4a456-138">value</span><span class="sxs-lookup"><span data-stu-id="4a456-138">value</span></span>|<span data-ttu-id="4a456-139">String</span><span class="sxs-lookup"><span data-stu-id="4a456-139">String</span></span>| <span data-ttu-id="4a456-140">在 OAuth 2.0 访问令牌中，资源应用程序应期望的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="4a456-140">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a456-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a456-141">JSON representation</span></span>
<span data-ttu-id="4a456-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a456-142">Here is a JSON representation of the resource.</span></span>

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
