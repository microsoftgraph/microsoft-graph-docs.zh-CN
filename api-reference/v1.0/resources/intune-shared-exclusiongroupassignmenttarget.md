---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fbfa4e6df9dae514a99fa96aace073bd702def9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523761"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="dcd54-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcd54-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="dcd54-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcd54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcd54-105">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="dcd54-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="dcd54-106">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="dcd54-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dcd54-107">属性</span><span class="sxs-lookup"><span data-stu-id="dcd54-107">Properties</span></span>
|<span data-ttu-id="dcd54-108">属性</span><span class="sxs-lookup"><span data-stu-id="dcd54-108">Property</span></span>|<span data-ttu-id="dcd54-109">类型</span><span class="sxs-lookup"><span data-stu-id="dcd54-109">Type</span></span>|<span data-ttu-id="dcd54-110">说明</span><span class="sxs-lookup"><span data-stu-id="dcd54-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcd54-111">groupId</span><span class="sxs-lookup"><span data-stu-id="dcd54-111">groupId</span></span>|<span data-ttu-id="dcd54-112">String</span><span class="sxs-lookup"><span data-stu-id="dcd54-112">String</span></span>|<span data-ttu-id="dcd54-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="dcd54-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="dcd54-114">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="dcd54-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcd54-115">关系</span><span class="sxs-lookup"><span data-stu-id="dcd54-115">Relationships</span></span>
<span data-ttu-id="dcd54-116">无</span><span class="sxs-lookup"><span data-stu-id="dcd54-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcd54-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcd54-117">JSON Representation</span></span>
<span data-ttu-id="dcd54-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcd54-118">Here is a JSON representation of the resource.</span></span>
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



