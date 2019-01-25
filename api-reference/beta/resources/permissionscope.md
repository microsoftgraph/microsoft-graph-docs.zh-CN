---
title: permissionScope 资源类型
description: 表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过 Application 对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **Oauth2Permissions**属性和应用程序实体的 ServicePrincipal 实体是**OAuth2Permission**的集合。
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517076"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="566f3-105">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="566f3-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="566f3-106">表示一个 OAuth 2.0 委派权限范围。</span><span class="sxs-lookup"><span data-stu-id="566f3-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="566f3-107">指定的 OAuth 2.0 委派的权限范围可能请求 （通过[Application](application.md)对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。</span><span class="sxs-lookup"><span data-stu-id="566f3-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="566f3-108">**Oauth2Permissions**属性和[应用程序](application.md)实体的[ServicePrincipal](serviceprincipal.md)实体是**OAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="566f3-108">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="566f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="566f3-109">Properties</span></span>

| <span data-ttu-id="566f3-110">属性</span><span class="sxs-lookup"><span data-stu-id="566f3-110">Property</span></span> | <span data-ttu-id="566f3-111">类型</span><span class="sxs-lookup"><span data-stu-id="566f3-111">Type</span></span> | <span data-ttu-id="566f3-112">说明</span><span class="sxs-lookup"><span data-stu-id="566f3-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="566f3-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="566f3-113">adminConsentDescription</span></span>|<span data-ttu-id="566f3-114">String</span><span class="sxs-lookup"><span data-stu-id="566f3-114">String</span></span>| <span data-ttu-id="566f3-115">权限管理员同意和应用程序分配体验中显示的帮助文本。</span><span class="sxs-lookup"><span data-stu-id="566f3-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="566f3-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="566f3-116">adminConsentDisplayName</span></span>|<span data-ttu-id="566f3-117">String</span><span class="sxs-lookup"><span data-stu-id="566f3-117">String</span></span>| <span data-ttu-id="566f3-118">权限管理的同意和应用程序分配体验中显示的的显示名称。</span><span class="sxs-lookup"><span data-stu-id="566f3-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="566f3-119">id</span><span class="sxs-lookup"><span data-stu-id="566f3-119">id</span></span>|<span data-ttu-id="566f3-120">Guid</span><span class="sxs-lookup"><span data-stu-id="566f3-120">Guid</span></span>| <span data-ttu-id="566f3-121">唯一范围权限 oauth2Permissions 集合内的标识符。</span><span class="sxs-lookup"><span data-stu-id="566f3-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="566f3-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="566f3-122">isEnabled</span></span>|<span data-ttu-id="566f3-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="566f3-123">Boolean</span></span>| <span data-ttu-id="566f3-124">在创建或更新权限，此属性必须设置为**true** （这是默认值）。</span><span class="sxs-lookup"><span data-stu-id="566f3-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="566f3-125">若要删除的权限，此属性必须先设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="566f3-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="566f3-126">此时，在后续呼叫，可能会删除权限。</span><span class="sxs-lookup"><span data-stu-id="566f3-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="566f3-127">Origin</span><span class="sxs-lookup"><span data-stu-id="566f3-127">origin</span></span>|<span data-ttu-id="566f3-128">String</span><span class="sxs-lookup"><span data-stu-id="566f3-128">String</span></span>| <span data-ttu-id="566f3-129">供内部使用。</span><span class="sxs-lookup"><span data-stu-id="566f3-129">For internal use.</span></span> |
|<span data-ttu-id="566f3-130">type</span><span class="sxs-lookup"><span data-stu-id="566f3-130">type</span></span>|<span data-ttu-id="566f3-131">String</span><span class="sxs-lookup"><span data-stu-id="566f3-131">String</span></span>| <span data-ttu-id="566f3-132">指定是否此范围权限可以同意由最终用户，或者是否必须由公司管理员同意租户级权限。</span><span class="sxs-lookup"><span data-stu-id="566f3-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="566f3-133">可能的值为*用户*或*管理员*。</span><span class="sxs-lookup"><span data-stu-id="566f3-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="566f3-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="566f3-134">userConsentDescription</span></span>|<span data-ttu-id="566f3-135">String</span><span class="sxs-lookup"><span data-stu-id="566f3-135">String</span></span>| <span data-ttu-id="566f3-136">权限帮助最终用户同意体验中显示的文本。</span><span class="sxs-lookup"><span data-stu-id="566f3-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="566f3-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="566f3-137">userConsentDisplayName</span></span>|<span data-ttu-id="566f3-138">String</span><span class="sxs-lookup"><span data-stu-id="566f3-138">String</span></span>| <span data-ttu-id="566f3-139">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="566f3-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="566f3-140">值</span><span class="sxs-lookup"><span data-stu-id="566f3-140">value</span></span>|<span data-ttu-id="566f3-141">String</span><span class="sxs-lookup"><span data-stu-id="566f3-141">String</span></span>| <span data-ttu-id="566f3-142">范围声明的资源应用程序应产生预期 OAuth 2.0 访问令牌中的值。</span><span class="sxs-lookup"><span data-stu-id="566f3-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="566f3-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="566f3-143">JSON representation</span></span>
<span data-ttu-id="566f3-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="566f3-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
