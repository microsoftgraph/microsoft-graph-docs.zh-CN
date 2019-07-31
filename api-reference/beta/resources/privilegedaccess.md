---
title: privilegedAccess 资源类型
description: " 例如, `privilegedAccess/azureResources`表示用于管理对 Azure 资源的权限访问的 PIM。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7f59f8420be6ff97511415e944d154cb5d59950f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965787"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="5d754-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d754-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d754-104">表示由特权标识管理 (PIM) 服务提供的一组功能。</span><span class="sxs-lookup"><span data-stu-id="5d754-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="5d754-105">表示由 PIM `privilegedAccess`管理的不同提供程序的不同实例;例如, `privilegedAccess/azureResources`表示用于管理对 Azure 资源的权限访问的 PIM。</span><span class="sxs-lookup"><span data-stu-id="5d754-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="5d754-106">`privilegedAccess`目前为只读。</span><span class="sxs-lookup"><span data-stu-id="5d754-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="5d754-107">`privilegedAccess`实体`POST`集`PUT`上`PATCH`不支持`DELETE` 、、或操作。</span><span class="sxs-lookup"><span data-stu-id="5d754-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="5d754-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d754-108">Properties</span></span>
| <span data-ttu-id="5d754-109">属性</span><span class="sxs-lookup"><span data-stu-id="5d754-109">Property</span></span>  | <span data-ttu-id="5d754-110">类型</span><span class="sxs-lookup"><span data-stu-id="5d754-110">Type</span></span>      |<span data-ttu-id="5d754-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d754-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="5d754-112">id</span><span class="sxs-lookup"><span data-stu-id="5d754-112">id</span></span>         |<span data-ttu-id="5d754-113">String</span><span class="sxs-lookup"><span data-stu-id="5d754-113">String</span></span>     |<span data-ttu-id="5d754-114">由 PIM 管理的提供程序的 id。</span><span class="sxs-lookup"><span data-stu-id="5d754-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="5d754-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5d754-115">displayName</span></span>|<span data-ttu-id="5d754-116">String</span><span class="sxs-lookup"><span data-stu-id="5d754-116">String</span></span>     |<span data-ttu-id="5d754-117">由 PIM 管理的提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5d754-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5d754-118">关系</span><span class="sxs-lookup"><span data-stu-id="5d754-118">Relationships</span></span>
| <span data-ttu-id="5d754-119">关系</span><span class="sxs-lookup"><span data-stu-id="5d754-119">Relationship</span></span>   | <span data-ttu-id="5d754-120">类型</span><span class="sxs-lookup"><span data-stu-id="5d754-120">Type</span></span>                                         |<span data-ttu-id="5d754-121">说明</span><span class="sxs-lookup"><span data-stu-id="5d754-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="5d754-122">resources</span><span class="sxs-lookup"><span data-stu-id="5d754-122">resources</span></span>       |<span data-ttu-id="5d754-123">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="5d754-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="5d754-124">提供程序的资源集合。</span><span class="sxs-lookup"><span data-stu-id="5d754-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="5d754-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="5d754-125">roleAssignments</span></span> |<span data-ttu-id="5d754-126">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5d754-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="5d754-127">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="5d754-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="5d754-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="5d754-128">roleDefinitions</span></span> |<span data-ttu-id="5d754-129">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="5d754-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="5d754-130">提供程序的角色 defintions 的集合。</span><span class="sxs-lookup"><span data-stu-id="5d754-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="5d754-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="5d754-131">roleAssignmentRequests</span></span> |<span data-ttu-id="5d754-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="5d754-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="5d754-133">提供程序的角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="5d754-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="5d754-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="5d754-134">roleSettings</span></span> |<span data-ttu-id="5d754-135">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="5d754-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="5d754-136">提供程序的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="5d754-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5d754-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d754-137">JSON representation</span></span>

<span data-ttu-id="5d754-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d754-138">Here is a JSON representation of the resource.</span></span>

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
