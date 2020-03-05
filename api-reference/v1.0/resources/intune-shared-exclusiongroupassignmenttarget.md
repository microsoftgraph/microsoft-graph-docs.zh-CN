---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08bf52ab16a29c869366373c5f205f25b352e1b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447841"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="cd0d4-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd0d4-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="cd0d4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cd0d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd0d4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd0d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd0d4-106">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="cd0d4-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="cd0d4-107">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="cd0d4-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cd0d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd0d4-108">Properties</span></span>
|<span data-ttu-id="cd0d4-109">属性</span><span class="sxs-lookup"><span data-stu-id="cd0d4-109">Property</span></span>|<span data-ttu-id="cd0d4-110">类型</span><span class="sxs-lookup"><span data-stu-id="cd0d4-110">Type</span></span>|<span data-ttu-id="cd0d4-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd0d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd0d4-112">groupId</span><span class="sxs-lookup"><span data-stu-id="cd0d4-112">groupId</span></span>|<span data-ttu-id="cd0d4-113">String</span><span class="sxs-lookup"><span data-stu-id="cd0d4-113">String</span></span>|<span data-ttu-id="cd0d4-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="cd0d4-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="cd0d4-115">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="cd0d4-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd0d4-116">关系</span><span class="sxs-lookup"><span data-stu-id="cd0d4-116">Relationships</span></span>
<span data-ttu-id="cd0d4-117">无</span><span class="sxs-lookup"><span data-stu-id="cd0d4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd0d4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd0d4-118">JSON Representation</span></span>
<span data-ttu-id="cd0d4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd0d4-119">Here is a JSON representation of the resource.</span></span>
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




