---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46297a1670136ffc1c7de07c4e4640121a50434
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967504"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="42694-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="42694-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="42694-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42694-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42694-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42694-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42694-106">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="42694-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="42694-107">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="42694-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42694-108">属性</span><span class="sxs-lookup"><span data-stu-id="42694-108">Properties</span></span>
|<span data-ttu-id="42694-109">属性</span><span class="sxs-lookup"><span data-stu-id="42694-109">Property</span></span>|<span data-ttu-id="42694-110">类型</span><span class="sxs-lookup"><span data-stu-id="42694-110">Type</span></span>|<span data-ttu-id="42694-111">说明</span><span class="sxs-lookup"><span data-stu-id="42694-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42694-112">groupId</span><span class="sxs-lookup"><span data-stu-id="42694-112">groupId</span></span>|<span data-ttu-id="42694-113">String</span><span class="sxs-lookup"><span data-stu-id="42694-113">String</span></span>|<span data-ttu-id="42694-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="42694-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42694-115">关系</span><span class="sxs-lookup"><span data-stu-id="42694-115">Relationships</span></span>
<span data-ttu-id="42694-116">无</span><span class="sxs-lookup"><span data-stu-id="42694-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42694-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42694-117">JSON Representation</span></span>
<span data-ttu-id="42694-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42694-118">Here is a JSON representation of the resource.</span></span>
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









