---
title: permissionScope 资源类型
description: 表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过 Application 对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **Oauth2Permissions**属性和应用程序实体的 ServicePrincipal 实体是**OAuth2Permission**的集合。
localization_priority: Normal
ms.openlocfilehash: a294316f5c6255d0873ce0dbe809c33dad89ae08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818149"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="203de-105">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="203de-105">permissionScope resource type</span></span>

> <span data-ttu-id="203de-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="203de-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="203de-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="203de-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="203de-108">表示一个 OAuth 2.0 委派权限范围。</span><span class="sxs-lookup"><span data-stu-id="203de-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="203de-109">指定的 OAuth 2.0 委派的权限范围可能请求 （通过[Application](application.md)对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。</span><span class="sxs-lookup"><span data-stu-id="203de-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="203de-110">**Oauth2Permissions**属性和[应用程序](application.md)实体的[ServicePrincipal](serviceprincipal.md)实体是**OAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="203de-110">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="203de-111">属性</span><span class="sxs-lookup"><span data-stu-id="203de-111">Properties</span></span>

| <span data-ttu-id="203de-112">属性</span><span class="sxs-lookup"><span data-stu-id="203de-112">Property</span></span> | <span data-ttu-id="203de-113">类型</span><span class="sxs-lookup"><span data-stu-id="203de-113">Type</span></span> | <span data-ttu-id="203de-114">Description</span><span class="sxs-lookup"><span data-stu-id="203de-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="203de-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="203de-115">adminConsentDescription</span></span>|<span data-ttu-id="203de-116">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-116">String</span></span>| <span data-ttu-id="203de-117">权限管理员同意和应用程序分配体验中显示的帮助文本。</span><span class="sxs-lookup"><span data-stu-id="203de-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="203de-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="203de-118">adminConsentDisplayName</span></span>|<span data-ttu-id="203de-119">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-119">String</span></span>| <span data-ttu-id="203de-120">权限管理的同意和应用程序分配体验中显示的的显示名称。</span><span class="sxs-lookup"><span data-stu-id="203de-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="203de-121">id</span><span class="sxs-lookup"><span data-stu-id="203de-121">id</span></span>|<span data-ttu-id="203de-122">Guid</span><span class="sxs-lookup"><span data-stu-id="203de-122">Guid</span></span>| <span data-ttu-id="203de-123">唯一范围权限 oauth2Permissions 集合内的标识符。</span><span class="sxs-lookup"><span data-stu-id="203de-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="203de-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="203de-124">isEnabled</span></span>|<span data-ttu-id="203de-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="203de-125">Boolean</span></span>| <span data-ttu-id="203de-126">在创建或更新权限，此属性必须设置为**true** （这是默认值）。</span><span class="sxs-lookup"><span data-stu-id="203de-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="203de-127">若要删除的权限，此属性必须先设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="203de-127">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="203de-128">此时，在后续呼叫，可能会删除权限。</span><span class="sxs-lookup"><span data-stu-id="203de-128">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="203de-129">来源</span><span class="sxs-lookup"><span data-stu-id="203de-129">origin</span></span>|<span data-ttu-id="203de-130">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-130">String</span></span>| <span data-ttu-id="203de-131">供内部使用。</span><span class="sxs-lookup"><span data-stu-id="203de-131">For internal use.</span></span> |
|<span data-ttu-id="203de-132">type</span><span class="sxs-lookup"><span data-stu-id="203de-132">type</span></span>|<span data-ttu-id="203de-133">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-133">String</span></span>| <span data-ttu-id="203de-134">指定是否此范围权限可以同意由最终用户，或者是否必须由公司管理员同意租户级权限。</span><span class="sxs-lookup"><span data-stu-id="203de-134">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="203de-135">可能的值为*用户*或*管理员*。</span><span class="sxs-lookup"><span data-stu-id="203de-135">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="203de-136">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="203de-136">userConsentDescription</span></span>|<span data-ttu-id="203de-137">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-137">String</span></span>| <span data-ttu-id="203de-138">权限帮助最终用户同意体验中显示的文本。</span><span class="sxs-lookup"><span data-stu-id="203de-138">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="203de-139">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="203de-139">userConsentDisplayName</span></span>|<span data-ttu-id="203de-140">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-140">String</span></span>| <span data-ttu-id="203de-141">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="203de-141">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="203de-142">值</span><span class="sxs-lookup"><span data-stu-id="203de-142">value</span></span>|<span data-ttu-id="203de-143">字符串</span><span class="sxs-lookup"><span data-stu-id="203de-143">String</span></span>| <span data-ttu-id="203de-144">范围声明的资源应用程序应产生预期 OAuth 2.0 访问令牌中的值。</span><span class="sxs-lookup"><span data-stu-id="203de-144">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="203de-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="203de-145">JSON representation</span></span>
<span data-ttu-id="203de-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="203de-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
