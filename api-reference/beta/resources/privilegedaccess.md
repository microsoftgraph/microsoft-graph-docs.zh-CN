---
title: privilegedAccess 资源类型
description: " 例如， `privilegedAccess/azureResources` 表示 PIM 管理对 Azure 资源的特权访问。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8a144ba13974a728b4e89fc661f34f20e8157689
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136617"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="67a71-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="67a71-103">privilegedAccess resource type</span></span>

<span data-ttu-id="67a71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67a71-105">表示由 PIM 服务特权标识 (提供的) 组。</span><span class="sxs-lookup"><span data-stu-id="67a71-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="67a71-106">不同的实例表示由 PIM 管理的不同提供程序;例如，表示 PIM 管理对 Azure 资源的 `privilegedAccess` `privilegedAccess/azureResources` 特权访问。</span><span class="sxs-lookup"><span data-stu-id="67a71-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="67a71-107">`privilegedAccess` 目前为只读。</span><span class="sxs-lookup"><span data-stu-id="67a71-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="67a71-108">实体 `POST` `PUT` 集不支持 、 或 `PATCH` `DELETE` `privilegedAccess` 操作。</span><span class="sxs-lookup"><span data-stu-id="67a71-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="67a71-109">属性</span><span class="sxs-lookup"><span data-stu-id="67a71-109">Properties</span></span>
| <span data-ttu-id="67a71-110">属性</span><span class="sxs-lookup"><span data-stu-id="67a71-110">Property</span></span>  | <span data-ttu-id="67a71-111">类型</span><span class="sxs-lookup"><span data-stu-id="67a71-111">Type</span></span>      |<span data-ttu-id="67a71-112">说明</span><span class="sxs-lookup"><span data-stu-id="67a71-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="67a71-113">id</span><span class="sxs-lookup"><span data-stu-id="67a71-113">id</span></span>         |<span data-ttu-id="67a71-114">字符串</span><span class="sxs-lookup"><span data-stu-id="67a71-114">String</span></span>     |<span data-ttu-id="67a71-115">由 PIM 管理的提供程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="67a71-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="67a71-116">displayName</span><span class="sxs-lookup"><span data-stu-id="67a71-116">displayName</span></span>|<span data-ttu-id="67a71-117">字符串</span><span class="sxs-lookup"><span data-stu-id="67a71-117">String</span></span>     |<span data-ttu-id="67a71-118">由显示名称 PIM 管理的提供程序的名称。</span><span class="sxs-lookup"><span data-stu-id="67a71-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="67a71-119">关系</span><span class="sxs-lookup"><span data-stu-id="67a71-119">Relationships</span></span>
| <span data-ttu-id="67a71-120">关系</span><span class="sxs-lookup"><span data-stu-id="67a71-120">Relationship</span></span>   | <span data-ttu-id="67a71-121">类型</span><span class="sxs-lookup"><span data-stu-id="67a71-121">Type</span></span>                                         |<span data-ttu-id="67a71-122">说明</span><span class="sxs-lookup"><span data-stu-id="67a71-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="67a71-123">resources</span><span class="sxs-lookup"><span data-stu-id="67a71-123">resources</span></span>       |<span data-ttu-id="67a71-124">[governanceResource](../resources/governanceresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a71-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="67a71-125">提供程序的资源集合。</span><span class="sxs-lookup"><span data-stu-id="67a71-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="67a71-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="67a71-126">roleAssignments</span></span> |<span data-ttu-id="67a71-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a71-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="67a71-128">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="67a71-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="67a71-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="67a71-129">roleDefinitions</span></span> |<span data-ttu-id="67a71-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a71-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="67a71-131">提供程序的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="67a71-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="67a71-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="67a71-132">roleAssignmentRequests</span></span> |<span data-ttu-id="67a71-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a71-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="67a71-134">提供程序角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="67a71-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="67a71-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="67a71-135">roleSettings</span></span> |<span data-ttu-id="67a71-136">[governanceRoleSetting](../resources/governancerolesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a71-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="67a71-137">提供程序的角色设置集合。</span><span class="sxs-lookup"><span data-stu-id="67a71-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="67a71-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67a71-138">JSON representation</span></span>

<span data-ttu-id="67a71-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67a71-139">Here is a JSON representation of the resource.</span></span>

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


