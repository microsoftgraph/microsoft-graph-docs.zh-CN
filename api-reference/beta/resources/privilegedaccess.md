---
title: privilegedAccess 资源类型
description: " 例如, `privilegedAccess/azureResources`表示用于管理对 Azure 资源的权限访问的 PIM。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563658"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="e8771-103">privilegedAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8771-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8771-104">表示由特权标识管理 (PIM) 服务提供的一组功能。</span><span class="sxs-lookup"><span data-stu-id="e8771-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="e8771-105">表示由 PIM `privilegedAccess`管理的不同提供程序的不同实例;例如, `privilegedAccess/azureResources`表示用于管理对 Azure 资源的权限访问的 PIM。</span><span class="sxs-lookup"><span data-stu-id="e8771-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="e8771-106">`privilegedAccess`目前为只读。</span><span class="sxs-lookup"><span data-stu-id="e8771-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="e8771-107">`privilegedAccess`实体`POST`集`PUT`上`PATCH`不支持`DELETE` 、、或操作。</span><span class="sxs-lookup"><span data-stu-id="e8771-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="e8771-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8771-108">Properties</span></span>
| <span data-ttu-id="e8771-109">属性</span><span class="sxs-lookup"><span data-stu-id="e8771-109">Property</span></span>  | <span data-ttu-id="e8771-110">类型</span><span class="sxs-lookup"><span data-stu-id="e8771-110">Type</span></span>      |<span data-ttu-id="e8771-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8771-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="e8771-112">id</span><span class="sxs-lookup"><span data-stu-id="e8771-112">id</span></span>         |<span data-ttu-id="e8771-113">String</span><span class="sxs-lookup"><span data-stu-id="e8771-113">String</span></span>     |<span data-ttu-id="e8771-114">由 PIM 管理的提供程序的 id。</span><span class="sxs-lookup"><span data-stu-id="e8771-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="e8771-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e8771-115">displayName</span></span>|<span data-ttu-id="e8771-116">String</span><span class="sxs-lookup"><span data-stu-id="e8771-116">String</span></span>     |<span data-ttu-id="e8771-117">由 PIM 管理的提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e8771-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e8771-118">关系</span><span class="sxs-lookup"><span data-stu-id="e8771-118">Relationships</span></span>
| <span data-ttu-id="e8771-119">关系</span><span class="sxs-lookup"><span data-stu-id="e8771-119">Relationship</span></span>   | <span data-ttu-id="e8771-120">类型</span><span class="sxs-lookup"><span data-stu-id="e8771-120">Type</span></span>                                         |<span data-ttu-id="e8771-121">说明</span><span class="sxs-lookup"><span data-stu-id="e8771-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="e8771-122">资源</span><span class="sxs-lookup"><span data-stu-id="e8771-122">resources</span></span>       |<span data-ttu-id="e8771-123">[governanceResource](../resources/governanceresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8771-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="e8771-124">提供程序的资源集合。</span><span class="sxs-lookup"><span data-stu-id="e8771-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="e8771-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="e8771-125">roleAssignments</span></span> |<span data-ttu-id="e8771-126">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8771-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="e8771-127">提供程序的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="e8771-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="e8771-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="e8771-128">roleDefinitions</span></span> |<span data-ttu-id="e8771-129">[governanceRoleDefinition](../resources/governanceroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8771-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="e8771-130">提供程序的角色 defintions 的集合。</span><span class="sxs-lookup"><span data-stu-id="e8771-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="e8771-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e8771-131">roleAssignmentRequests</span></span> |<span data-ttu-id="e8771-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8771-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="e8771-133">提供程序的角色分配请求的集合。</span><span class="sxs-lookup"><span data-stu-id="e8771-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="e8771-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="e8771-134">roleSettings</span></span> |<span data-ttu-id="e8771-135">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8771-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="e8771-136">提供程序的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="e8771-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e8771-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8771-137">JSON representation</span></span>

<span data-ttu-id="e8771-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8771-138">Here is a JSON representation of the resource.</span></span>

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
