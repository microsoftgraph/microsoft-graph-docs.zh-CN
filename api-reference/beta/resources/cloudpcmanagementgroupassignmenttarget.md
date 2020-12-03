---
title: cloudPcManagementGroupAssignmentTarget 资源类型
description: 代表工作分配目标组的复杂类型。 基本类型： CloudPcManagementAssignmentTarget
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5216b15a97484bf58d2e2d621dbc26435f180be4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563843"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a><span data-ttu-id="c236b-104">cloudPcManagementGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="c236b-104">cloudPcManagementGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="c236b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c236b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c236b-106">代表工作分配目标组的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="c236b-106">Complex type that represents the assignment target group.</span></span>
<span data-ttu-id="c236b-107">继承自 [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="c236b-107">Inherits from [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="c236b-108">属性</span><span class="sxs-lookup"><span data-stu-id="c236b-108">Properties</span></span>

|<span data-ttu-id="c236b-109">属性</span><span class="sxs-lookup"><span data-stu-id="c236b-109">Property</span></span>|<span data-ttu-id="c236b-110">类型</span><span class="sxs-lookup"><span data-stu-id="c236b-110">Type</span></span>|<span data-ttu-id="c236b-111">说明</span><span class="sxs-lookup"><span data-stu-id="c236b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c236b-112">groupId</span><span class="sxs-lookup"><span data-stu-id="c236b-112">groupId</span></span>|<span data-ttu-id="c236b-113">String</span><span class="sxs-lookup"><span data-stu-id="c236b-113">String</span></span>|<span data-ttu-id="c236b-114">工作分配的目标组的 id</span><span class="sxs-lookup"><span data-stu-id="c236b-114">The id of the assignment's target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="c236b-115">关系</span><span class="sxs-lookup"><span data-stu-id="c236b-115">Relationships</span></span>

<span data-ttu-id="c236b-116">无。</span><span class="sxs-lookup"><span data-stu-id="c236b-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c236b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c236b-117">JSON representation</span></span>

<span data-ttu-id="c236b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c236b-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.cloudPcManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcManagementGroupAssignmentTarget",
  "groupId": "String"
}
```
