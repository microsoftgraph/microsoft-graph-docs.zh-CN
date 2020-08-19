---
title: privilegedAccess 资源类型
description: " 例如， `privilegedAccess/azureResources` 表示用于管理对 Azure 资源的权限访问的 PIM。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: c57dd911d105ba4d096a09f9262b847db5240fa1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811448"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="867b8-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="867b8-103">privilegedAccess resource type</span></span>

<span data-ttu-id="867b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="867b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="867b8-105">表示由特权身份管理 (PIM) 服务提供的一组功能。</span><span class="sxs-lookup"><span data-stu-id="867b8-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="867b8-106">`privilegedAccess`表示由 PIM 管理的不同提供程序的不同实例; 例如， `privilegedAccess/azureResources` 表示用于管理对 Azure 资源的权限访问的 PIM。</span><span class="sxs-lookup"><span data-stu-id="867b8-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="867b8-107">`privilegedAccess` 目前为只读。</span><span class="sxs-lookup"><span data-stu-id="867b8-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="867b8-108">`POST` `PUT` `PATCH` `DELETE` 实体集上不支持、、或操作 `privilegedAccess` 。</span><span class="sxs-lookup"><span data-stu-id="867b8-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="867b8-109">属性</span><span class="sxs-lookup"><span data-stu-id="867b8-109">Properties</span></span>
| <span data-ttu-id="867b8-110">属性</span><span class="sxs-lookup"><span data-stu-id="867b8-110">Property</span></span>  | <span data-ttu-id="867b8-111">类型</span><span class="sxs-lookup"><span data-stu-id="867b8-111">Type</span></span>      |<span data-ttu-id="867b8-112">说明</span><span class="sxs-lookup"><span data-stu-id="867b8-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="867b8-113">id</span><span class="sxs-lookup"><span data-stu-id="867b8-113">id</span></span>         |<span data-ttu-id="867b8-114">String</span><span class="sxs-lookup"><span data-stu-id="867b8-114">String</span></span>     |<span data-ttu-id="867b8-115">由 PIM 管理的提供程序的 id。</span><span class="sxs-lookup"><span data-stu-id="867b8-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="867b8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="867b8-116">displayName</span></span>|<span data-ttu-id="867b8-117">String</span><span class="sxs-lookup"><span data-stu-id="867b8-117">String</span></span>     |<span data-ttu-id="867b8-118">由 PIM 管理的提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="867b8-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="867b8-119">关系</span><span class="sxs-lookup"><span data-stu-id="867b8-119">Relationships</span></span>
| <span data-ttu-id="867b8-120">关系</span><span class="sxs-lookup"><span data-stu-id="867b8-120">Relationship</span></span>   | <span data-ttu-id="867b8-121">类型</span><span class="sxs-lookup"><span data-stu-id="867b8-121">Type</span></span>                                         |<span data-ttu-id="867b8-122">说明</span><span class="sxs-lookup"><span data-stu-id="867b8-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="867b8-123">resources</span><span class="sxs-lookup"><span data-stu-id="867b8-123">resources</span></span>       |<span data-ttu-id="867b8-124">[governanceResource](../resources/governanceresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="867b8-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="867b8-125">提供程序的资源集合。</span><span class="sxs-lookup"><span data-stu-id="867b8-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="867b8-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="867b8-126">roleAssignments</span></span> |<span data-ttu-id="867b8-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="867b8-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="867b8-128">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="867b8-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="867b8-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="867b8-129">roleDefinitions</span></span> |<span data-ttu-id="867b8-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="867b8-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="867b8-131">提供程序的角色 defintions 的集合。</span><span class="sxs-lookup"><span data-stu-id="867b8-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="867b8-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="867b8-132">roleAssignmentRequests</span></span> |<span data-ttu-id="867b8-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="867b8-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="867b8-134">提供程序的角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="867b8-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="867b8-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="867b8-135">roleSettings</span></span> |<span data-ttu-id="867b8-136">[governanceRoleSetting](../resources/governancerolesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="867b8-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="867b8-137">提供程序的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="867b8-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="867b8-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="867b8-138">JSON representation</span></span>

<span data-ttu-id="867b8-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="867b8-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
