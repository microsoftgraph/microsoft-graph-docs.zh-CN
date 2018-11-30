---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
ms.openlocfilehash: fdbb463687d75791965db2ef05abfea1a269d1a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010257"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="157c0-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="157c0-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="157c0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="157c0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="157c0-105">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="157c0-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="157c0-106">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="157c0-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="157c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="157c0-107">Properties</span></span>
|<span data-ttu-id="157c0-108">属性</span><span class="sxs-lookup"><span data-stu-id="157c0-108">Property</span></span>|<span data-ttu-id="157c0-109">类型</span><span class="sxs-lookup"><span data-stu-id="157c0-109">Type</span></span>|<span data-ttu-id="157c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="157c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157c0-111">groupId</span><span class="sxs-lookup"><span data-stu-id="157c0-111">groupId</span></span>|<span data-ttu-id="157c0-112">String</span><span class="sxs-lookup"><span data-stu-id="157c0-112">String</span></span>|<span data-ttu-id="157c0-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="157c0-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="157c0-114">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="157c0-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="157c0-115">关系</span><span class="sxs-lookup"><span data-stu-id="157c0-115">Relationships</span></span>
<span data-ttu-id="157c0-116">无</span><span class="sxs-lookup"><span data-stu-id="157c0-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="157c0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="157c0-117">JSON Representation</span></span>
<span data-ttu-id="157c0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="157c0-118">Here is a JSON representation of the resource.</span></span>
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



