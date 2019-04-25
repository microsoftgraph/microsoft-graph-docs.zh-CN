---
title: appRole 资源类型
description: 表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 servicePrincipal 实体和 application 实体的**appRoles**属性是**appRole**的集合。
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535700"
---
# <a name="approle-resource-type"></a><span data-ttu-id="75a42-104">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="75a42-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75a42-105">表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="75a42-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="75a42-106">[servicePrincipal](serviceprincipal.md)实体和[application](application.md)实体的**appRoles**属性是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="75a42-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="75a42-107">重要说明: 当前版本中禁用了此功能。</span><span class="sxs-lookup"><span data-stu-id="75a42-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75a42-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75a42-108">JSON representation</span></span>

<span data-ttu-id="75a42-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75a42-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="75a42-110">属性</span><span class="sxs-lookup"><span data-stu-id="75a42-110">Properties</span></span>
| <span data-ttu-id="75a42-111">属性</span><span class="sxs-lookup"><span data-stu-id="75a42-111">Property</span></span>     | <span data-ttu-id="75a42-112">类型</span><span class="sxs-lookup"><span data-stu-id="75a42-112">Type</span></span>   |<span data-ttu-id="75a42-113">说明</span><span class="sxs-lookup"><span data-stu-id="75a42-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75a42-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="75a42-114">allowedMemberTypes</span></span>|<span data-ttu-id="75a42-115">String collection</span><span class="sxs-lookup"><span data-stu-id="75a42-115">String collection</span></span>|<span data-ttu-id="75a42-116">指定是否可以通过设置为 "用户" 或将此应用程序角色定义分配给用户和组, 或通过设置为 "应用程序" 或同时设置为 "应用程序" 来将此应用程序角色定义分配给用户和组。</span><span class="sxs-lookup"><span data-stu-id="75a42-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="75a42-117">description</span><span class="sxs-lookup"><span data-stu-id="75a42-117">description</span></span>|<span data-ttu-id="75a42-118">String</span><span class="sxs-lookup"><span data-stu-id="75a42-118">String</span></span>|<span data-ttu-id="75a42-119">在管理员应用分配和同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="75a42-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="75a42-120">displayName</span><span class="sxs-lookup"><span data-stu-id="75a42-120">displayName</span></span>|<span data-ttu-id="75a42-121">字符串</span><span class="sxs-lookup"><span data-stu-id="75a42-121">String</span></span>|<span data-ttu-id="75a42-122">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="75a42-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="75a42-123">id</span><span class="sxs-lookup"><span data-stu-id="75a42-123">id</span></span>|<span data-ttu-id="75a42-124">Guid</span><span class="sxs-lookup"><span data-stu-id="75a42-124">Guid</span></span>|<span data-ttu-id="75a42-125">**appRoles**集合中的唯一角色标识符。</span><span class="sxs-lookup"><span data-stu-id="75a42-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="75a42-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="75a42-126">isEnabled</span></span>|<span data-ttu-id="75a42-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a42-127">Boolean</span></span>|<span data-ttu-id="75a42-128">在创建或更新角色定义时, 必须将其设置为**true** (默认值)。</span><span class="sxs-lookup"><span data-stu-id="75a42-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="75a42-129">若要删除角色, 必须首先将此设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="75a42-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="75a42-130">此时, 在后续调用中, 可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="75a42-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="75a42-131">value</span><span class="sxs-lookup"><span data-stu-id="75a42-131">value</span></span>|<span data-ttu-id="75a42-132">String</span><span class="sxs-lookup"><span data-stu-id="75a42-132">String</span></span>|<span data-ttu-id="75a42-133">指定应用程序应在身份验证和访问令牌中预期的角色声明的值。</span><span class="sxs-lookup"><span data-stu-id="75a42-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

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
