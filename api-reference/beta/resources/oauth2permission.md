---
title: oAuth2Permission 资源类型
description: 表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过 application 对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **AppRoles**属性和应用程序实体的 servicePrincipal 实体是**oAuth2Permission**的集合。
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510811"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="e56d6-105">oAuth2Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="e56d6-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e56d6-106">表示一个 OAuth 2.0 委派权限范围。</span><span class="sxs-lookup"><span data-stu-id="e56d6-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="e56d6-107">指定的 OAuth 2.0 委派的权限范围可能请求 （通过[application](application.md)对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。</span><span class="sxs-lookup"><span data-stu-id="e56d6-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="e56d6-108">**AppRoles**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**oAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="e56d6-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e56d6-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e56d6-109">JSON representation</span></span>

<span data-ttu-id="e56d6-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e56d6-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e56d6-111">属性</span><span class="sxs-lookup"><span data-stu-id="e56d6-111">Properties</span></span>
| <span data-ttu-id="e56d6-112">属性</span><span class="sxs-lookup"><span data-stu-id="e56d6-112">Property</span></span>     | <span data-ttu-id="e56d6-113">类型</span><span class="sxs-lookup"><span data-stu-id="e56d6-113">Type</span></span>   |<span data-ttu-id="e56d6-114">说明</span><span class="sxs-lookup"><span data-stu-id="e56d6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e56d6-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="e56d6-115">adminConsentDescription</span></span>|<span data-ttu-id="e56d6-116">String</span><span class="sxs-lookup"><span data-stu-id="e56d6-116">String</span></span>|<span data-ttu-id="e56d6-117">权限管理员同意和应用程序分配体验中显示的帮助文本。</span><span class="sxs-lookup"><span data-stu-id="e56d6-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="e56d6-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="e56d6-118">adminConsentDisplayName</span></span>|<span data-ttu-id="e56d6-119">String</span><span class="sxs-lookup"><span data-stu-id="e56d6-119">String</span></span>|<span data-ttu-id="e56d6-120">权限管理的同意和应用程序分配体验中显示的的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e56d6-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="e56d6-121">id</span><span class="sxs-lookup"><span data-stu-id="e56d6-121">id</span></span>|<span data-ttu-id="e56d6-122">Guid</span><span class="sxs-lookup"><span data-stu-id="e56d6-122">Guid</span></span>|<span data-ttu-id="e56d6-123">唯一范围权限 oauth2Permissions 集合内的标识符。</span><span class="sxs-lookup"><span data-stu-id="e56d6-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="e56d6-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e56d6-124">isEnabled</span></span>|<span data-ttu-id="e56d6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e56d6-125">Boolean</span></span>|<span data-ttu-id="e56d6-126">在创建或更新权限，此属性必须设置为**true** （这是默认值）。</span><span class="sxs-lookup"><span data-stu-id="e56d6-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="e56d6-127">若要删除的权限，此属性必须先设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="e56d6-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="e56d6-128">此时，在后续呼叫，可能会删除权限。</span><span class="sxs-lookup"><span data-stu-id="e56d6-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="e56d6-129">type</span><span class="sxs-lookup"><span data-stu-id="e56d6-129">type</span></span>|<span data-ttu-id="e56d6-130">String</span><span class="sxs-lookup"><span data-stu-id="e56d6-130">String</span></span>|<span data-ttu-id="e56d6-131">指定是否此范围权限可以同意由最终用户，或者是否必须同意公司管理员通过租户级权限。</span><span class="sxs-lookup"><span data-stu-id="e56d6-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="e56d6-132">可能的值为"用户"或"管理员"。</span><span class="sxs-lookup"><span data-stu-id="e56d6-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="e56d6-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="e56d6-133">userConsentDescription</span></span>|<span data-ttu-id="e56d6-134">String</span><span class="sxs-lookup"><span data-stu-id="e56d6-134">String</span></span>|<span data-ttu-id="e56d6-135">权限帮助最终用户同意体验中显示的文本。</span><span class="sxs-lookup"><span data-stu-id="e56d6-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="e56d6-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="e56d6-136">userConsentDisplayName</span></span>|<span data-ttu-id="e56d6-137">String</span><span class="sxs-lookup"><span data-stu-id="e56d6-137">String</span></span>|<span data-ttu-id="e56d6-138">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e56d6-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="e56d6-139">值</span><span class="sxs-lookup"><span data-stu-id="e56d6-139">value</span></span>|<span data-ttu-id="e56d6-140">String</span><span class="sxs-lookup"><span data-stu-id="e56d6-140">String</span></span>|<span data-ttu-id="e56d6-141">范围声明的资源应用程序应产生预期 OAuth 2.0 访问令牌中的值。</span><span class="sxs-lookup"><span data-stu-id="e56d6-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
