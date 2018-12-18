---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: tfitzmac
ms.openlocfilehash: 6dbcb5cd55fcddd22fdf205d7fc8fc50e6b397c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319794"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="87591-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="87591-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="87591-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="87591-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87591-105">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="87591-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="87591-106">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="87591-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="87591-107">属性</span><span class="sxs-lookup"><span data-stu-id="87591-107">Properties</span></span>
|<span data-ttu-id="87591-108">属性</span><span class="sxs-lookup"><span data-stu-id="87591-108">Property</span></span>|<span data-ttu-id="87591-109">类型</span><span class="sxs-lookup"><span data-stu-id="87591-109">Type</span></span>|<span data-ttu-id="87591-110">说明</span><span class="sxs-lookup"><span data-stu-id="87591-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87591-111">groupId</span><span class="sxs-lookup"><span data-stu-id="87591-111">groupId</span></span>|<span data-ttu-id="87591-112">String</span><span class="sxs-lookup"><span data-stu-id="87591-112">String</span></span>|<span data-ttu-id="87591-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="87591-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87591-114">关系</span><span class="sxs-lookup"><span data-stu-id="87591-114">Relationships</span></span>
<span data-ttu-id="87591-115">无</span><span class="sxs-lookup"><span data-stu-id="87591-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87591-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87591-116">JSON Representation</span></span>
<span data-ttu-id="87591-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87591-117">Here is a JSON representation of the resource.</span></span>
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



