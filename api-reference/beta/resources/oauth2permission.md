---
title: oAuth2Permission 资源类型
description: 表示 OAuth 2.0 委派的权限范围。 调用资源应用程序时, 客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围 (通过 application 对象上的**requiredResourceAccess**集合)。 ServicePrincipal 实体和 application 实体的**appRoles**属性是**oAuth2Permission**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16dfa93d13127d585cd5b56a56987bb22ab39d8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009571"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="be270-105">oAuth2Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="be270-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be270-106">表示 OAuth 2.0 委派的权限范围。</span><span class="sxs-lookup"><span data-stu-id="be270-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="be270-107">调用资源应用程序时, 客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围 (通过[application](application.md)对象上的**requiredResourceAccess**集合)。</span><span class="sxs-lookup"><span data-stu-id="be270-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="be270-108">[ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**appRoles**属性是**oAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="be270-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="be270-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be270-109">JSON representation</span></span>

<span data-ttu-id="be270-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be270-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="be270-111">属性</span><span class="sxs-lookup"><span data-stu-id="be270-111">Properties</span></span>
| <span data-ttu-id="be270-112">属性</span><span class="sxs-lookup"><span data-stu-id="be270-112">Property</span></span>     | <span data-ttu-id="be270-113">类型</span><span class="sxs-lookup"><span data-stu-id="be270-113">Type</span></span>   |<span data-ttu-id="be270-114">说明</span><span class="sxs-lookup"><span data-stu-id="be270-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be270-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="be270-115">adminConsentDescription</span></span>|<span data-ttu-id="be270-116">String</span><span class="sxs-lookup"><span data-stu-id="be270-116">String</span></span>|<span data-ttu-id="be270-117">管理员同意和应用工作分配体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="be270-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="be270-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="be270-118">adminConsentDisplayName</span></span>|<span data-ttu-id="be270-119">String</span><span class="sxs-lookup"><span data-stu-id="be270-119">String</span></span>|<span data-ttu-id="be270-120">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be270-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="be270-121">id</span><span class="sxs-lookup"><span data-stu-id="be270-121">id</span></span>|<span data-ttu-id="be270-122">Guid</span><span class="sxs-lookup"><span data-stu-id="be270-122">Guid</span></span>|<span data-ttu-id="be270-123">Oauth2Permissions 集合中的唯一作用域权限标识符。</span><span class="sxs-lookup"><span data-stu-id="be270-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="be270-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="be270-124">isEnabled</span></span>|<span data-ttu-id="be270-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="be270-125">Boolean</span></span>|<span data-ttu-id="be270-126">在创建或更新权限时, 此属性必须设置为**true** (默认值)。</span><span class="sxs-lookup"><span data-stu-id="be270-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="be270-127">若要删除权限, 必须首先将此属性设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="be270-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="be270-128">此时, 在后续调用中, 可能会删除该权限。</span><span class="sxs-lookup"><span data-stu-id="be270-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="be270-129">type</span><span class="sxs-lookup"><span data-stu-id="be270-129">type</span></span>|<span data-ttu-id="be270-130">String</span><span class="sxs-lookup"><span data-stu-id="be270-130">String</span></span>|<span data-ttu-id="be270-131">指定此范围权限是否可由最终用户许可, 或者是否为公司管理员必须同意的租户范围内的权限。</span><span class="sxs-lookup"><span data-stu-id="be270-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="be270-132">可能的值为 "User" 或 "Admin"。</span><span class="sxs-lookup"><span data-stu-id="be270-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="be270-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="be270-133">userConsentDescription</span></span>|<span data-ttu-id="be270-134">String</span><span class="sxs-lookup"><span data-stu-id="be270-134">String</span></span>|<span data-ttu-id="be270-135">最终用户同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="be270-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="be270-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="be270-136">userConsentDisplayName</span></span>|<span data-ttu-id="be270-137">String</span><span class="sxs-lookup"><span data-stu-id="be270-137">String</span></span>|<span data-ttu-id="be270-138">最终用户同意体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be270-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="be270-139">value</span><span class="sxs-lookup"><span data-stu-id="be270-139">value</span></span>|<span data-ttu-id="be270-140">String</span><span class="sxs-lookup"><span data-stu-id="be270-140">String</span></span>|<span data-ttu-id="be270-141">在 OAuth 2.0 访问令牌中, 资源应用程序应期望的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="be270-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
