---
title: appRole 资源类型
description: 表示应用程序角色调用另一个应用程序的客户端应用程序可能请求的或可能用于分配给用户或组指定的应用程序角色中的应用程序。 **AppRoles**属性和应用程序实体的 servicePrincipal 实体是**appRole**的集合。
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640411"
---
# <a name="approle-resource-type"></a><span data-ttu-id="392ea-104">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="392ea-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="392ea-105">表示应用程序角色调用另一个应用程序的客户端应用程序可能请求的或可能用于分配给用户或组指定的应用程序角色中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="392ea-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="392ea-106">**AppRoles**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="392ea-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="392ea-107">重要说明： 此功能在当前版本中已禁用。</span><span class="sxs-lookup"><span data-stu-id="392ea-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="392ea-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="392ea-108">JSON representation</span></span>

<span data-ttu-id="392ea-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="392ea-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="392ea-110">属性</span><span class="sxs-lookup"><span data-stu-id="392ea-110">Properties</span></span>
| <span data-ttu-id="392ea-111">属性</span><span class="sxs-lookup"><span data-stu-id="392ea-111">Property</span></span>     | <span data-ttu-id="392ea-112">类型</span><span class="sxs-lookup"><span data-stu-id="392ea-112">Type</span></span>   |<span data-ttu-id="392ea-113">说明</span><span class="sxs-lookup"><span data-stu-id="392ea-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="392ea-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="392ea-114">allowedMemberTypes</span></span>|<span data-ttu-id="392ea-115">String collection</span><span class="sxs-lookup"><span data-stu-id="392ea-115">String collection</span></span>|<span data-ttu-id="392ea-116">指定此应用程序角色定义可以设置为"User"，或其他应用程序 （即正在访问此端口监控程序服务方案中的应用程序） 分配给用户和组设置到"应用程序"，或两者。</span><span class="sxs-lookup"><span data-stu-id="392ea-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="392ea-117">description</span><span class="sxs-lookup"><span data-stu-id="392ea-117">description</span></span>|<span data-ttu-id="392ea-118">String</span><span class="sxs-lookup"><span data-stu-id="392ea-118">String</span></span>|<span data-ttu-id="392ea-119">权限帮助管理应用程序分配中显示的文本和同意体验。</span><span class="sxs-lookup"><span data-stu-id="392ea-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="392ea-120">displayName</span><span class="sxs-lookup"><span data-stu-id="392ea-120">displayName</span></span>|<span data-ttu-id="392ea-121">String</span><span class="sxs-lookup"><span data-stu-id="392ea-121">String</span></span>|<span data-ttu-id="392ea-122">权限管理的同意和应用程序分配体验中显示的的显示名称。</span><span class="sxs-lookup"><span data-stu-id="392ea-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="392ea-123">id</span><span class="sxs-lookup"><span data-stu-id="392ea-123">id</span></span>|<span data-ttu-id="392ea-124">Guid</span><span class="sxs-lookup"><span data-stu-id="392ea-124">Guid</span></span>|<span data-ttu-id="392ea-125">**AppRoles**集合内的独有角色标识符。</span><span class="sxs-lookup"><span data-stu-id="392ea-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="392ea-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="392ea-126">isEnabled</span></span>|<span data-ttu-id="392ea-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="392ea-127">Boolean</span></span>|<span data-ttu-id="392ea-128">当创建或更新一个角色定义，这必须设置为**true** （这是默认值）。</span><span class="sxs-lookup"><span data-stu-id="392ea-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="392ea-129">若要删除一个角色，这必须先设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="392ea-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="392ea-130">此时，在后续呼叫，可以删除此角色。</span><span class="sxs-lookup"><span data-stu-id="392ea-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="392ea-131">值</span><span class="sxs-lookup"><span data-stu-id="392ea-131">value</span></span>|<span data-ttu-id="392ea-132">String</span><span class="sxs-lookup"><span data-stu-id="392ea-132">String</span></span>|<span data-ttu-id="392ea-133">身份验证和访问令牌中指定应用程序应产生预期角色声明的值。</span><span class="sxs-lookup"><span data-stu-id="392ea-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
