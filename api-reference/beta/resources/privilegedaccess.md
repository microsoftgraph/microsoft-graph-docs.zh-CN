---
title: privilegedAccess 资源类型
description: " 例如， `privilegedAccess/azureResources` 表示用于管理对 Azure 资源的权限访问的 PIM。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: f815228157721f6100af79f53f84abf43763f632
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070630"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="ade2b-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="ade2b-103">privilegedAccess resource type</span></span>

<span data-ttu-id="ade2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ade2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade2b-105">表示由特权身份管理 (PIM) 服务提供的一组功能。</span><span class="sxs-lookup"><span data-stu-id="ade2b-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="ade2b-106">`privilegedAccess`表示由 PIM 管理的不同提供程序的不同实例; 例如， `privilegedAccess/azureResources` 表示用于管理对 Azure 资源的权限访问的 PIM。</span><span class="sxs-lookup"><span data-stu-id="ade2b-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="ade2b-107">`privilegedAccess` 目前为只读。</span><span class="sxs-lookup"><span data-stu-id="ade2b-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="ade2b-108">`POST` `PUT` `PATCH` `DELETE` 实体集上不支持、、或操作 `privilegedAccess` 。</span><span class="sxs-lookup"><span data-stu-id="ade2b-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="ade2b-109">属性</span><span class="sxs-lookup"><span data-stu-id="ade2b-109">Properties</span></span>
| <span data-ttu-id="ade2b-110">属性</span><span class="sxs-lookup"><span data-stu-id="ade2b-110">Property</span></span>  | <span data-ttu-id="ade2b-111">类型</span><span class="sxs-lookup"><span data-stu-id="ade2b-111">Type</span></span>      |<span data-ttu-id="ade2b-112">说明</span><span class="sxs-lookup"><span data-stu-id="ade2b-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="ade2b-113">id</span><span class="sxs-lookup"><span data-stu-id="ade2b-113">id</span></span>         |<span data-ttu-id="ade2b-114">String</span><span class="sxs-lookup"><span data-stu-id="ade2b-114">String</span></span>     |<span data-ttu-id="ade2b-115">由 PIM 管理的提供程序的 id。</span><span class="sxs-lookup"><span data-stu-id="ade2b-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="ade2b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="ade2b-116">displayName</span></span>|<span data-ttu-id="ade2b-117">String</span><span class="sxs-lookup"><span data-stu-id="ade2b-117">String</span></span>     |<span data-ttu-id="ade2b-118">由 PIM 管理的提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ade2b-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="ade2b-119">关系</span><span class="sxs-lookup"><span data-stu-id="ade2b-119">Relationships</span></span>
| <span data-ttu-id="ade2b-120">关系</span><span class="sxs-lookup"><span data-stu-id="ade2b-120">Relationship</span></span>   | <span data-ttu-id="ade2b-121">类型</span><span class="sxs-lookup"><span data-stu-id="ade2b-121">Type</span></span>                                         |<span data-ttu-id="ade2b-122">说明</span><span class="sxs-lookup"><span data-stu-id="ade2b-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="ade2b-123">resources</span><span class="sxs-lookup"><span data-stu-id="ade2b-123">resources</span></span>       |<span data-ttu-id="ade2b-124">[governanceResource](../resources/governanceresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade2b-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="ade2b-125">提供程序的资源集合。</span><span class="sxs-lookup"><span data-stu-id="ade2b-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="ade2b-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="ade2b-126">roleAssignments</span></span> |<span data-ttu-id="ade2b-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade2b-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="ade2b-128">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="ade2b-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="ade2b-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ade2b-129">roleDefinitions</span></span> |<span data-ttu-id="ade2b-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade2b-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="ade2b-131">提供程序的角色 defintions 的集合。</span><span class="sxs-lookup"><span data-stu-id="ade2b-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="ade2b-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="ade2b-132">roleAssignmentRequests</span></span> |<span data-ttu-id="ade2b-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade2b-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="ade2b-134">提供程序的角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="ade2b-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="ade2b-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="ade2b-135">roleSettings</span></span> |<span data-ttu-id="ade2b-136">[governanceRoleSetting](../resources/governancerolesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade2b-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="ade2b-137">提供程序的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="ade2b-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ade2b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ade2b-138">JSON representation</span></span>

<span data-ttu-id="ade2b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade2b-139">Here is a JSON representation of the resource.</span></span>

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


