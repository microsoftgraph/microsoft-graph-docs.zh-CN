---
title: privilegedAccess 资源类型
description: " 例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512925"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="6b75b-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b75b-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b75b-104">代表一组特权标识管理 (PIM) 服务提供的功能。</span><span class="sxs-lookup"><span data-stu-id="6b75b-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="6b75b-105">不同实例`privilegedAccess`表示不同的提供程序托管的 PIM;例如，`privilegedAccess/azureResources`代表 PIM 管理特权 Azure 资源的访问。</span><span class="sxs-lookup"><span data-stu-id="6b75b-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="6b75b-106">`privilegedAccess`现在是只读的。</span><span class="sxs-lookup"><span data-stu-id="6b75b-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="6b75b-107">不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`privilegedAccess`实体集。</span><span class="sxs-lookup"><span data-stu-id="6b75b-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="6b75b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b75b-108">Properties</span></span>
| <span data-ttu-id="6b75b-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b75b-109">Property</span></span>  | <span data-ttu-id="6b75b-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b75b-110">Type</span></span>      |<span data-ttu-id="6b75b-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b75b-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="6b75b-112">id</span><span class="sxs-lookup"><span data-stu-id="6b75b-112">id</span></span>         |<span data-ttu-id="6b75b-113">String</span><span class="sxs-lookup"><span data-stu-id="6b75b-113">String</span></span>     |<span data-ttu-id="6b75b-114">由 PIM 管理提供程序的 id。</span><span class="sxs-lookup"><span data-stu-id="6b75b-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="6b75b-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6b75b-115">displayName</span></span>|<span data-ttu-id="6b75b-116">String</span><span class="sxs-lookup"><span data-stu-id="6b75b-116">String</span></span>     |<span data-ttu-id="6b75b-117">由 PIM 管理提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6b75b-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="6b75b-118">关系</span><span class="sxs-lookup"><span data-stu-id="6b75b-118">Relationships</span></span>
| <span data-ttu-id="6b75b-119">关系</span><span class="sxs-lookup"><span data-stu-id="6b75b-119">Relationship</span></span>   | <span data-ttu-id="6b75b-120">类型</span><span class="sxs-lookup"><span data-stu-id="6b75b-120">Type</span></span>                                         |<span data-ttu-id="6b75b-121">说明</span><span class="sxs-lookup"><span data-stu-id="6b75b-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="6b75b-122">resources</span><span class="sxs-lookup"><span data-stu-id="6b75b-122">resources</span></span>       |<span data-ttu-id="6b75b-123">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="6b75b-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="6b75b-124">提供程序的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="6b75b-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="6b75b-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="6b75b-125">roleAssignments</span></span> |<span data-ttu-id="6b75b-126">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="6b75b-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="6b75b-127">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="6b75b-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="6b75b-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="6b75b-128">roleDefinitions</span></span> |<span data-ttu-id="6b75b-129">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="6b75b-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="6b75b-130">提供程序的角色定义的集合。</span><span class="sxs-lookup"><span data-stu-id="6b75b-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="6b75b-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="6b75b-131">roleAssignmentRequests</span></span> |<span data-ttu-id="6b75b-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="6b75b-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="6b75b-133">角色提供程序的工作分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="6b75b-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="6b75b-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="6b75b-134">roleSettings</span></span> |<span data-ttu-id="6b75b-135">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="6b75b-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="6b75b-136">角色提供程序的设置的集合。</span><span class="sxs-lookup"><span data-stu-id="6b75b-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6b75b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b75b-137">JSON representation</span></span>

<span data-ttu-id="6b75b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b75b-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
