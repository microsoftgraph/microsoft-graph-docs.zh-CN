---
title: oAuth2Permission 资源类型
description: 表示 OAuth 2.0 委派的权限范围。 调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过 application 对象上的**requiredResourceAccess**集合）。 ServicePrincipal 实体和 application 实体的**appRoles**属性是**oAuth2Permission**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d17834e3cbfcc1d22c9531befe7baa29215f8c4f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522538"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="65dd9-105">oAuth2Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="65dd9-105">oAuth2Permission resource type</span></span>

<span data-ttu-id="65dd9-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="65dd9-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65dd9-107">表示 OAuth 2.0 委派的权限范围。</span><span class="sxs-lookup"><span data-stu-id="65dd9-107">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="65dd9-108">调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过[application](application.md)对象上的**requiredResourceAccess**集合）。</span><span class="sxs-lookup"><span data-stu-id="65dd9-108">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="65dd9-109">[ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**appRoles**属性是**oAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="65dd9-109">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="65dd9-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65dd9-110">JSON representation</span></span>

<span data-ttu-id="65dd9-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65dd9-111">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="65dd9-112">属性</span><span class="sxs-lookup"><span data-stu-id="65dd9-112">Properties</span></span>
| <span data-ttu-id="65dd9-113">属性</span><span class="sxs-lookup"><span data-stu-id="65dd9-113">Property</span></span>     | <span data-ttu-id="65dd9-114">类型</span><span class="sxs-lookup"><span data-stu-id="65dd9-114">Type</span></span>   |<span data-ttu-id="65dd9-115">说明</span><span class="sxs-lookup"><span data-stu-id="65dd9-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65dd9-116">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="65dd9-116">adminConsentDescription</span></span>|<span data-ttu-id="65dd9-117">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-117">String</span></span>|<span data-ttu-id="65dd9-118">管理员同意和应用工作分配体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="65dd9-118">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="65dd9-119">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="65dd9-119">adminConsentDisplayName</span></span>|<span data-ttu-id="65dd9-120">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-120">String</span></span>|<span data-ttu-id="65dd9-121">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="65dd9-121">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="65dd9-122">id</span><span class="sxs-lookup"><span data-stu-id="65dd9-122">id</span></span>|<span data-ttu-id="65dd9-123">Guid</span><span class="sxs-lookup"><span data-stu-id="65dd9-123">Guid</span></span>|<span data-ttu-id="65dd9-124">Oauth2Permissions 集合中的唯一作用域权限标识符。</span><span class="sxs-lookup"><span data-stu-id="65dd9-124">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="65dd9-125">isEnabled</span><span class="sxs-lookup"><span data-stu-id="65dd9-125">isEnabled</span></span>|<span data-ttu-id="65dd9-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="65dd9-126">Boolean</span></span>|<span data-ttu-id="65dd9-127">在创建或更新权限时，此属性必须设置为**true** （默认值）。</span><span class="sxs-lookup"><span data-stu-id="65dd9-127">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="65dd9-128">若要删除权限，必须首先将此属性设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="65dd9-128">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="65dd9-129">此时，在后续调用中，可能会删除该权限。</span><span class="sxs-lookup"><span data-stu-id="65dd9-129">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="65dd9-130">type</span><span class="sxs-lookup"><span data-stu-id="65dd9-130">type</span></span>|<span data-ttu-id="65dd9-131">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-131">String</span></span>|<span data-ttu-id="65dd9-132">指定此范围权限是否可由最终用户许可，或者是否为公司管理员必须同意的租户范围内的权限。</span><span class="sxs-lookup"><span data-stu-id="65dd9-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="65dd9-133">可能的值为 "User" 或 "Admin"。</span><span class="sxs-lookup"><span data-stu-id="65dd9-133">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="65dd9-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="65dd9-134">userConsentDescription</span></span>|<span data-ttu-id="65dd9-135">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-135">String</span></span>|<span data-ttu-id="65dd9-136">最终用户同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="65dd9-136">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="65dd9-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="65dd9-137">userConsentDisplayName</span></span>|<span data-ttu-id="65dd9-138">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-138">String</span></span>|<span data-ttu-id="65dd9-139">最终用户同意体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="65dd9-139">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="65dd9-140">value</span><span class="sxs-lookup"><span data-stu-id="65dd9-140">value</span></span>|<span data-ttu-id="65dd9-141">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-141">String</span></span>|<span data-ttu-id="65dd9-142">在 OAuth 2.0 访问令牌中，资源应用程序应期望的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="65dd9-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

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
