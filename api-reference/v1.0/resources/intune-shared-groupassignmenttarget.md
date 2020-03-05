---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f103315cc0c0499545a7fe3adb8bc31f9d24880
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447834"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="efe44-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="efe44-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="efe44-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="efe44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efe44-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efe44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe44-106">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="efe44-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="efe44-107">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="efe44-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efe44-108">属性</span><span class="sxs-lookup"><span data-stu-id="efe44-108">Properties</span></span>
|<span data-ttu-id="efe44-109">属性</span><span class="sxs-lookup"><span data-stu-id="efe44-109">Property</span></span>|<span data-ttu-id="efe44-110">类型</span><span class="sxs-lookup"><span data-stu-id="efe44-110">Type</span></span>|<span data-ttu-id="efe44-111">说明</span><span class="sxs-lookup"><span data-stu-id="efe44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe44-112">groupId</span><span class="sxs-lookup"><span data-stu-id="efe44-112">groupId</span></span>|<span data-ttu-id="efe44-113">String</span><span class="sxs-lookup"><span data-stu-id="efe44-113">String</span></span>|<span data-ttu-id="efe44-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="efe44-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efe44-115">关系</span><span class="sxs-lookup"><span data-stu-id="efe44-115">Relationships</span></span>
<span data-ttu-id="efe44-116">无</span><span class="sxs-lookup"><span data-stu-id="efe44-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efe44-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efe44-117">JSON Representation</span></span>
<span data-ttu-id="efe44-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efe44-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```




