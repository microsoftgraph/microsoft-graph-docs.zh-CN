---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 390c9de591af10dc19df7bc989b9fa01ef59f86a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527430"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="82662-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="82662-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="82662-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82662-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82662-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82662-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82662-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82662-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82662-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="82662-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="82662-108">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="82662-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82662-109">属性</span><span class="sxs-lookup"><span data-stu-id="82662-109">Properties</span></span>
|<span data-ttu-id="82662-110">属性</span><span class="sxs-lookup"><span data-stu-id="82662-110">Property</span></span>|<span data-ttu-id="82662-111">类型</span><span class="sxs-lookup"><span data-stu-id="82662-111">Type</span></span>|<span data-ttu-id="82662-112">说明</span><span class="sxs-lookup"><span data-stu-id="82662-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82662-113">groupId</span><span class="sxs-lookup"><span data-stu-id="82662-113">groupId</span></span>|<span data-ttu-id="82662-114">String</span><span class="sxs-lookup"><span data-stu-id="82662-114">String</span></span>|<span data-ttu-id="82662-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="82662-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="82662-116">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="82662-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="82662-117">关系</span><span class="sxs-lookup"><span data-stu-id="82662-117">Relationships</span></span>
<span data-ttu-id="82662-118">无</span><span class="sxs-lookup"><span data-stu-id="82662-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82662-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82662-119">JSON Representation</span></span>
<span data-ttu-id="82662-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82662-120">Here is a JSON representation of the resource.</span></span>
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



