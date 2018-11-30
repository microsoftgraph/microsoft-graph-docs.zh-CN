---
title: oAuth2Permission 资源类型
description: 表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过 application 对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **AppRoles**属性和应用程序实体的 servicePrincipal 实体是**oAuth2Permission**的集合。
ms.openlocfilehash: 4a790c935dd84fb7bd4e1422ca59914d9a319ae9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046965"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="4ff83-105">oAuth2Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ff83-105">oAuth2Permission resource type</span></span>

> <span data-ttu-id="4ff83-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ff83-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ff83-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ff83-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ff83-108">表示一个 OAuth 2.0 委派权限范围。</span><span class="sxs-lookup"><span data-stu-id="4ff83-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="4ff83-109">指定的 OAuth 2.0 委派的权限范围可能请求 （通过[application](application.md)对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。</span><span class="sxs-lookup"><span data-stu-id="4ff83-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="4ff83-110">**AppRoles**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**oAuth2Permission**的集合。</span><span class="sxs-lookup"><span data-stu-id="4ff83-110">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4ff83-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ff83-111">JSON representation</span></span>

<span data-ttu-id="4ff83-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ff83-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4ff83-113">属性</span><span class="sxs-lookup"><span data-stu-id="4ff83-113">Properties</span></span>
| <span data-ttu-id="4ff83-114">属性</span><span class="sxs-lookup"><span data-stu-id="4ff83-114">Property</span></span>     | <span data-ttu-id="4ff83-115">类型</span><span class="sxs-lookup"><span data-stu-id="4ff83-115">Type</span></span>   |<span data-ttu-id="4ff83-116">说明</span><span class="sxs-lookup"><span data-stu-id="4ff83-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ff83-117">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="4ff83-117">adminConsentDescription</span></span>|<span data-ttu-id="4ff83-118">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff83-118">String</span></span>|<span data-ttu-id="4ff83-119">权限管理员同意和应用程序分配体验中显示的帮助文本。</span><span class="sxs-lookup"><span data-stu-id="4ff83-119">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4ff83-120">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="4ff83-120">adminConsentDisplayName</span></span>|<span data-ttu-id="4ff83-121">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff83-121">String</span></span>|<span data-ttu-id="4ff83-122">权限管理的同意和应用程序分配体验中显示的的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4ff83-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4ff83-123">id</span><span class="sxs-lookup"><span data-stu-id="4ff83-123">id</span></span>|<span data-ttu-id="4ff83-124">Guid</span><span class="sxs-lookup"><span data-stu-id="4ff83-124">Guid</span></span>|<span data-ttu-id="4ff83-125">唯一范围权限 oauth2Permissions 集合内的标识符。</span><span class="sxs-lookup"><span data-stu-id="4ff83-125">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="4ff83-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4ff83-126">isEnabled</span></span>|<span data-ttu-id="4ff83-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ff83-127">Boolean</span></span>|<span data-ttu-id="4ff83-128">在创建或更新权限，此属性必须设置为**true** （这是默认值）。</span><span class="sxs-lookup"><span data-stu-id="4ff83-128">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="4ff83-129">若要删除的权限，此属性必须先设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="4ff83-129">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="4ff83-130">此时，在后续呼叫，可能会删除权限。</span><span class="sxs-lookup"><span data-stu-id="4ff83-130">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="4ff83-131">type</span><span class="sxs-lookup"><span data-stu-id="4ff83-131">type</span></span>|<span data-ttu-id="4ff83-132">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff83-132">String</span></span>|<span data-ttu-id="4ff83-133">指定是否此范围权限可以同意由最终用户，或者是否必须同意公司管理员通过租户级权限。</span><span class="sxs-lookup"><span data-stu-id="4ff83-133">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="4ff83-134">可能的值为"用户"或"管理员"。</span><span class="sxs-lookup"><span data-stu-id="4ff83-134">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="4ff83-135">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="4ff83-135">userConsentDescription</span></span>|<span data-ttu-id="4ff83-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff83-136">String</span></span>|<span data-ttu-id="4ff83-137">权限帮助最终用户同意体验中显示的文本。</span><span class="sxs-lookup"><span data-stu-id="4ff83-137">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="4ff83-138">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="4ff83-138">userConsentDisplayName</span></span>|<span data-ttu-id="4ff83-139">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff83-139">String</span></span>|<span data-ttu-id="4ff83-140">显示在最终用户同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4ff83-140">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="4ff83-141">值</span><span class="sxs-lookup"><span data-stu-id="4ff83-141">value</span></span>|<span data-ttu-id="4ff83-142">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff83-142">String</span></span>|<span data-ttu-id="4ff83-143">范围声明的资源应用程序应产生预期 OAuth 2.0 访问令牌中的值。</span><span class="sxs-lookup"><span data-stu-id="4ff83-143">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
