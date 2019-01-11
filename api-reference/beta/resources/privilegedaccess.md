---
title: privilegedAccess 资源类型
description: " 例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。"
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810050"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="fdb15-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdb15-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="fdb15-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fdb15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdb15-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fdb15-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdb15-106">代表一组特权标识管理 (PIM) 服务提供的功能。</span><span class="sxs-lookup"><span data-stu-id="fdb15-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="fdb15-107">不同实例`privilegedAccess`表示不同的提供程序托管的 PIM;例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。</span><span class="sxs-lookup"><span data-stu-id="fdb15-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="fdb15-108">`privilegedAccess`现在是只读的。</span><span class="sxs-lookup"><span data-stu-id="fdb15-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="fdb15-109">不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`privilegedAccess`实体集。</span><span class="sxs-lookup"><span data-stu-id="fdb15-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="fdb15-110">属性</span><span class="sxs-lookup"><span data-stu-id="fdb15-110">Properties</span></span>
| <span data-ttu-id="fdb15-111">属性</span><span class="sxs-lookup"><span data-stu-id="fdb15-111">Property</span></span>  | <span data-ttu-id="fdb15-112">类型</span><span class="sxs-lookup"><span data-stu-id="fdb15-112">Type</span></span>      |<span data-ttu-id="fdb15-113">说明</span><span class="sxs-lookup"><span data-stu-id="fdb15-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="fdb15-114">id</span><span class="sxs-lookup"><span data-stu-id="fdb15-114">id</span></span>         |<span data-ttu-id="fdb15-115">字符串</span><span class="sxs-lookup"><span data-stu-id="fdb15-115">String</span></span>     |<span data-ttu-id="fdb15-116">由 PIM 管理提供程序的 id。</span><span class="sxs-lookup"><span data-stu-id="fdb15-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="fdb15-117">displayName</span><span class="sxs-lookup"><span data-stu-id="fdb15-117">displayName</span></span>|<span data-ttu-id="fdb15-118">字符串</span><span class="sxs-lookup"><span data-stu-id="fdb15-118">String</span></span>     |<span data-ttu-id="fdb15-119">由 PIM 管理提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fdb15-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="fdb15-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="fdb15-120">Relationships</span></span>
| <span data-ttu-id="fdb15-121">关系</span><span class="sxs-lookup"><span data-stu-id="fdb15-121">Relationship</span></span>   | <span data-ttu-id="fdb15-122">类型</span><span class="sxs-lookup"><span data-stu-id="fdb15-122">Type</span></span>                                         |<span data-ttu-id="fdb15-123">Description</span><span class="sxs-lookup"><span data-stu-id="fdb15-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="fdb15-124">resources</span><span class="sxs-lookup"><span data-stu-id="fdb15-124">resources</span></span>       |<span data-ttu-id="fdb15-125">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdb15-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="fdb15-126">提供程序的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb15-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="fdb15-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="fdb15-127">roleAssignments</span></span> |<span data-ttu-id="fdb15-128">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdb15-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="fdb15-129">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb15-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="fdb15-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="fdb15-130">roleDefinitions</span></span> |<span data-ttu-id="fdb15-131">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdb15-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="fdb15-132">提供程序的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb15-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="fdb15-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="fdb15-133">roleAssignmentRequests</span></span> |<span data-ttu-id="fdb15-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdb15-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="fdb15-135">角色提供程序的工作分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb15-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="fdb15-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="fdb15-136">roleSettings</span></span> |<span data-ttu-id="fdb15-137">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdb15-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="fdb15-138">角色提供程序的设置的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb15-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fdb15-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdb15-139">JSON representation</span></span>

<span data-ttu-id="fdb15-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdb15-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
