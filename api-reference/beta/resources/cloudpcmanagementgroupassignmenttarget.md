---
title: cloudPcManagementGroupAssignmentTarget 资源类型
description: 代表工作分配目标组的复杂类型。 基本类型： CloudPcManagementAssignmentTarget
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a6d046452bb3e9944712746ec7ef72914737186
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378326"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a><span data-ttu-id="878f7-104">cloudPcManagementGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="878f7-104">cloudPcManagementGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="878f7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="878f7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="878f7-106">代表工作分配目标组的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="878f7-106">Complex type that represents the assignment target group.</span></span>
<span data-ttu-id="878f7-107">继承自 [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="878f7-107">Inherits from [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="878f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="878f7-108">Properties</span></span>

|<span data-ttu-id="878f7-109">属性</span><span class="sxs-lookup"><span data-stu-id="878f7-109">Property</span></span>|<span data-ttu-id="878f7-110">类型</span><span class="sxs-lookup"><span data-stu-id="878f7-110">Type</span></span>|<span data-ttu-id="878f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="878f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="878f7-112">groupId</span><span class="sxs-lookup"><span data-stu-id="878f7-112">groupId</span></span>|<span data-ttu-id="878f7-113">String</span><span class="sxs-lookup"><span data-stu-id="878f7-113">String</span></span>|<span data-ttu-id="878f7-114">工作分配的目标组的 id</span><span class="sxs-lookup"><span data-stu-id="878f7-114">The id of the assignment's target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="878f7-115">关系</span><span class="sxs-lookup"><span data-stu-id="878f7-115">Relationships</span></span>

<span data-ttu-id="878f7-116">无。</span><span class="sxs-lookup"><span data-stu-id="878f7-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="878f7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="878f7-117">JSON representation</span></span>

<span data-ttu-id="878f7-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="878f7-118">The following is a JSON representation of the resource.</span></span>
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
