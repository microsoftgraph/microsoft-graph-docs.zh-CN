---
title: appRole 资源类型
description: 表示应用程序角色调用另一个应用程序的客户端应用程序可能请求的或可能用于分配给用户或组指定的应用程序角色中的应用程序。 **AppRoles**属性和应用程序实体的 servicePrincipal 实体是**appRole**的集合。
localization_priority: Normal
ms.openlocfilehash: 26fe11fc4f0c362de002c205c7e3b95a6ec4a314
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891544"
---
# <a name="approle-resource-type"></a><span data-ttu-id="3d871-104">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d871-104">appRole resource type</span></span>

> <span data-ttu-id="3d871-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3d871-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d871-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d871-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d871-107">表示应用程序角色调用另一个应用程序的客户端应用程序可能请求的或可能用于分配给用户或组指定的应用程序角色中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3d871-107">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="3d871-108">**AppRoles**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="3d871-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="3d871-109">重要说明： 此功能在当前版本中已禁用。</span><span class="sxs-lookup"><span data-stu-id="3d871-109">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d871-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d871-110">JSON representation</span></span>

<span data-ttu-id="3d871-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d871-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3d871-112">属性</span><span class="sxs-lookup"><span data-stu-id="3d871-112">Properties</span></span>
| <span data-ttu-id="3d871-113">属性</span><span class="sxs-lookup"><span data-stu-id="3d871-113">Property</span></span>     | <span data-ttu-id="3d871-114">类型</span><span class="sxs-lookup"><span data-stu-id="3d871-114">Type</span></span>   |<span data-ttu-id="3d871-115">Description</span><span class="sxs-lookup"><span data-stu-id="3d871-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d871-116">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="3d871-116">allowedMemberTypes</span></span>|<span data-ttu-id="3d871-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="3d871-117">String collection</span></span>|<span data-ttu-id="3d871-118">指定此应用程序角色定义可以设置为"User"，或其他应用程序 （即正在访问此端口监控程序服务方案中的应用程序） 分配给用户和组设置到"应用程序"，或两者。</span><span class="sxs-lookup"><span data-stu-id="3d871-118">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="3d871-119">说明</span><span class="sxs-lookup"><span data-stu-id="3d871-119">description</span></span>|<span data-ttu-id="3d871-120">字符串</span><span class="sxs-lookup"><span data-stu-id="3d871-120">String</span></span>|<span data-ttu-id="3d871-121">权限帮助管理应用程序分配中显示的文本和同意体验。</span><span class="sxs-lookup"><span data-stu-id="3d871-121">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="3d871-122">displayName</span><span class="sxs-lookup"><span data-stu-id="3d871-122">displayName</span></span>|<span data-ttu-id="3d871-123">字符串</span><span class="sxs-lookup"><span data-stu-id="3d871-123">String</span></span>|<span data-ttu-id="3d871-124">权限管理的同意和应用程序分配体验中显示的的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3d871-124">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="3d871-125">id</span><span class="sxs-lookup"><span data-stu-id="3d871-125">id</span></span>|<span data-ttu-id="3d871-126">Guid</span><span class="sxs-lookup"><span data-stu-id="3d871-126">Guid</span></span>|<span data-ttu-id="3d871-127">**AppRoles**集合内的独有角色标识符。</span><span class="sxs-lookup"><span data-stu-id="3d871-127">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="3d871-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3d871-128">isEnabled</span></span>|<span data-ttu-id="3d871-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d871-129">Boolean</span></span>|<span data-ttu-id="3d871-130">当创建或更新一个角色定义，这必须设置为**true** （这是默认值）。</span><span class="sxs-lookup"><span data-stu-id="3d871-130">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="3d871-131">若要删除一个角色，这必须先设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="3d871-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="3d871-132">此时，在后续呼叫，可以删除此角色。</span><span class="sxs-lookup"><span data-stu-id="3d871-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="3d871-133">值</span><span class="sxs-lookup"><span data-stu-id="3d871-133">value</span></span>|<span data-ttu-id="3d871-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3d871-134">String</span></span>|<span data-ttu-id="3d871-135">身份验证和访问令牌中指定应用程序应产生预期角色声明的值。</span><span class="sxs-lookup"><span data-stu-id="3d871-135">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
