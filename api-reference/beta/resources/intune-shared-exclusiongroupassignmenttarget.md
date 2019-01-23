---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a42cab192a9cd643c6c11de596ca0790fa8b4a5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421884"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="c3e67-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3e67-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c3e67-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c3e67-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3e67-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3e67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3e67-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3e67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3e67-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="c3e67-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="c3e67-108">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c3e67-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3e67-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3e67-109">Properties</span></span>
|<span data-ttu-id="c3e67-110">属性</span><span class="sxs-lookup"><span data-stu-id="c3e67-110">Property</span></span>|<span data-ttu-id="c3e67-111">类型</span><span class="sxs-lookup"><span data-stu-id="c3e67-111">Type</span></span>|<span data-ttu-id="c3e67-112">说明</span><span class="sxs-lookup"><span data-stu-id="c3e67-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e67-113">groupId</span><span class="sxs-lookup"><span data-stu-id="c3e67-113">groupId</span></span>|<span data-ttu-id="c3e67-114">String</span><span class="sxs-lookup"><span data-stu-id="c3e67-114">String</span></span>|<span data-ttu-id="c3e67-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="c3e67-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="c3e67-116">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c3e67-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3e67-117">关系</span><span class="sxs-lookup"><span data-stu-id="c3e67-117">Relationships</span></span>
<span data-ttu-id="c3e67-118">无</span><span class="sxs-lookup"><span data-stu-id="c3e67-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3e67-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3e67-119">JSON Representation</span></span>
<span data-ttu-id="c3e67-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3e67-120">Here is a JSON representation of the resource.</span></span>
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




