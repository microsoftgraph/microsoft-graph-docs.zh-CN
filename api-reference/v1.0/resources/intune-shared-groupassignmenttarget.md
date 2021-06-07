---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d90440ee70ad701b3bb19f159cda53a1355fc7f0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756762"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="22769-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="22769-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="22769-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22769-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22769-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22769-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22769-106">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="22769-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="22769-107">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="22769-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22769-108">属性</span><span class="sxs-lookup"><span data-stu-id="22769-108">Properties</span></span>
|<span data-ttu-id="22769-109">属性</span><span class="sxs-lookup"><span data-stu-id="22769-109">Property</span></span>|<span data-ttu-id="22769-110">类型</span><span class="sxs-lookup"><span data-stu-id="22769-110">Type</span></span>|<span data-ttu-id="22769-111">Description</span><span class="sxs-lookup"><span data-stu-id="22769-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22769-112">groupId</span><span class="sxs-lookup"><span data-stu-id="22769-112">groupId</span></span>|<span data-ttu-id="22769-113">String</span><span class="sxs-lookup"><span data-stu-id="22769-113">String</span></span>|<span data-ttu-id="22769-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="22769-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22769-115">关系</span><span class="sxs-lookup"><span data-stu-id="22769-115">Relationships</span></span>
<span data-ttu-id="22769-116">无</span><span class="sxs-lookup"><span data-stu-id="22769-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22769-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22769-117">JSON Representation</span></span>
<span data-ttu-id="22769-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22769-118">Here is a JSON representation of the resource.</span></span>
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




