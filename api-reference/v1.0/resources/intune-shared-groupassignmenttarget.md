---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
ms.openlocfilehash: 0ebb41b1f737a20a37d322bac7ab5ae6ab2a248f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009882"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2d975-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d975-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="2d975-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2d975-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d975-105">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="2d975-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="2d975-106">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2d975-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2d975-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d975-107">Properties</span></span>
|<span data-ttu-id="2d975-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d975-108">Property</span></span>|<span data-ttu-id="2d975-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d975-109">Type</span></span>|<span data-ttu-id="2d975-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d975-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d975-111">groupId</span><span class="sxs-lookup"><span data-stu-id="2d975-111">groupId</span></span>|<span data-ttu-id="2d975-112">String</span><span class="sxs-lookup"><span data-stu-id="2d975-112">String</span></span>|<span data-ttu-id="2d975-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="2d975-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d975-114">关系</span><span class="sxs-lookup"><span data-stu-id="2d975-114">Relationships</span></span>
<span data-ttu-id="2d975-115">无</span><span class="sxs-lookup"><span data-stu-id="2d975-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d975-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d975-116">JSON Representation</span></span>
<span data-ttu-id="2d975-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d975-117">Here is a JSON representation of the resource.</span></span>
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



