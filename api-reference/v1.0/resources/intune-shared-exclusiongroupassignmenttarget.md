---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb7cd456b3a70bff2ea9d6e1de693d14f91205b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751256"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="464eb-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="464eb-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="464eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="464eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="464eb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="464eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="464eb-106">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="464eb-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="464eb-107">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="464eb-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="464eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="464eb-108">Properties</span></span>
|<span data-ttu-id="464eb-109">属性</span><span class="sxs-lookup"><span data-stu-id="464eb-109">Property</span></span>|<span data-ttu-id="464eb-110">类型</span><span class="sxs-lookup"><span data-stu-id="464eb-110">Type</span></span>|<span data-ttu-id="464eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="464eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="464eb-112">groupId</span><span class="sxs-lookup"><span data-stu-id="464eb-112">groupId</span></span>|<span data-ttu-id="464eb-113">String</span><span class="sxs-lookup"><span data-stu-id="464eb-113">String</span></span>|<span data-ttu-id="464eb-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="464eb-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="464eb-115">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="464eb-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="464eb-116">关系</span><span class="sxs-lookup"><span data-stu-id="464eb-116">Relationships</span></span>
<span data-ttu-id="464eb-117">无</span><span class="sxs-lookup"><span data-stu-id="464eb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="464eb-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="464eb-118">JSON Representation</span></span>
<span data-ttu-id="464eb-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="464eb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```




