---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85da1976d4935e6cc8e2ca4d3d3e08e2ddd007ac
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770072"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="63505-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="63505-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="63505-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63505-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63505-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63505-106">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="63505-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="63505-107">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="63505-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63505-108">属性</span><span class="sxs-lookup"><span data-stu-id="63505-108">Properties</span></span>
|<span data-ttu-id="63505-109">属性</span><span class="sxs-lookup"><span data-stu-id="63505-109">Property</span></span>|<span data-ttu-id="63505-110">类型</span><span class="sxs-lookup"><span data-stu-id="63505-110">Type</span></span>|<span data-ttu-id="63505-111">说明</span><span class="sxs-lookup"><span data-stu-id="63505-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63505-112">groupId</span><span class="sxs-lookup"><span data-stu-id="63505-112">groupId</span></span>|<span data-ttu-id="63505-113">String</span><span class="sxs-lookup"><span data-stu-id="63505-113">String</span></span>|<span data-ttu-id="63505-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="63505-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63505-115">关系</span><span class="sxs-lookup"><span data-stu-id="63505-115">Relationships</span></span>
<span data-ttu-id="63505-116">无</span><span class="sxs-lookup"><span data-stu-id="63505-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63505-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63505-117">JSON Representation</span></span>
<span data-ttu-id="63505-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63505-118">Here is a JSON representation of the resource.</span></span>
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



