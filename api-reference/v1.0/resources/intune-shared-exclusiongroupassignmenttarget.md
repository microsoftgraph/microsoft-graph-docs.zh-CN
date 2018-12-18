---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: tfitzmac
ms.openlocfilehash: 8193ac714f7f68dc371454c809c3eaa3176f8453
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304512"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="cee8b-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="cee8b-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="cee8b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cee8b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cee8b-105">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="cee8b-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="cee8b-106">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="cee8b-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cee8b-107">属性</span><span class="sxs-lookup"><span data-stu-id="cee8b-107">Properties</span></span>
|<span data-ttu-id="cee8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cee8b-108">Property</span></span>|<span data-ttu-id="cee8b-109">类型</span><span class="sxs-lookup"><span data-stu-id="cee8b-109">Type</span></span>|<span data-ttu-id="cee8b-110">说明</span><span class="sxs-lookup"><span data-stu-id="cee8b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee8b-111">groupId</span><span class="sxs-lookup"><span data-stu-id="cee8b-111">groupId</span></span>|<span data-ttu-id="cee8b-112">String</span><span class="sxs-lookup"><span data-stu-id="cee8b-112">String</span></span>|<span data-ttu-id="cee8b-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="cee8b-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="cee8b-114">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="cee8b-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cee8b-115">关系</span><span class="sxs-lookup"><span data-stu-id="cee8b-115">Relationships</span></span>
<span data-ttu-id="cee8b-116">无</span><span class="sxs-lookup"><span data-stu-id="cee8b-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cee8b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cee8b-117">JSON Representation</span></span>
<span data-ttu-id="cee8b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cee8b-118">Here is a JSON representation of the resource.</span></span>
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



