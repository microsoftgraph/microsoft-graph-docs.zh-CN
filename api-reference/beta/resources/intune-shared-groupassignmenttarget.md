---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b15df3fab9303f56e697eb09305db50d3ddea8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523672"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="fa284-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa284-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="fa284-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fa284-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa284-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa284-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa284-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa284-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa284-107">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="fa284-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="fa284-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fa284-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa284-109">属性</span><span class="sxs-lookup"><span data-stu-id="fa284-109">Properties</span></span>
|<span data-ttu-id="fa284-110">属性</span><span class="sxs-lookup"><span data-stu-id="fa284-110">Property</span></span>|<span data-ttu-id="fa284-111">类型</span><span class="sxs-lookup"><span data-stu-id="fa284-111">Type</span></span>|<span data-ttu-id="fa284-112">说明</span><span class="sxs-lookup"><span data-stu-id="fa284-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa284-113">groupId</span><span class="sxs-lookup"><span data-stu-id="fa284-113">groupId</span></span>|<span data-ttu-id="fa284-114">String</span><span class="sxs-lookup"><span data-stu-id="fa284-114">String</span></span>|<span data-ttu-id="fa284-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="fa284-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa284-116">关系</span><span class="sxs-lookup"><span data-stu-id="fa284-116">Relationships</span></span>
<span data-ttu-id="fa284-117">无</span><span class="sxs-lookup"><span data-stu-id="fa284-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa284-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa284-118">JSON Representation</span></span>
<span data-ttu-id="fa284-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa284-119">Here is a JSON representation of the resource.</span></span>
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



