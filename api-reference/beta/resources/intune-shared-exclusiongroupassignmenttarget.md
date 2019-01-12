---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24e732bc0c48c9c25f35da1afbccef04d17fe0cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919860"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="a629f-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="a629f-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="a629f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a629f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a629f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a629f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a629f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a629f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a629f-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="a629f-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="a629f-108">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a629f-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a629f-109">属性</span><span class="sxs-lookup"><span data-stu-id="a629f-109">Properties</span></span>
|<span data-ttu-id="a629f-110">属性</span><span class="sxs-lookup"><span data-stu-id="a629f-110">Property</span></span>|<span data-ttu-id="a629f-111">类型</span><span class="sxs-lookup"><span data-stu-id="a629f-111">Type</span></span>|<span data-ttu-id="a629f-112">说明</span><span class="sxs-lookup"><span data-stu-id="a629f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a629f-113">groupId</span><span class="sxs-lookup"><span data-stu-id="a629f-113">groupId</span></span>|<span data-ttu-id="a629f-114">String</span><span class="sxs-lookup"><span data-stu-id="a629f-114">String</span></span>|<span data-ttu-id="a629f-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="a629f-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="a629f-116">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a629f-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a629f-117">关系</span><span class="sxs-lookup"><span data-stu-id="a629f-117">Relationships</span></span>
<span data-ttu-id="a629f-118">无</span><span class="sxs-lookup"><span data-stu-id="a629f-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a629f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a629f-119">JSON Representation</span></span>
<span data-ttu-id="a629f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a629f-120">Here is a JSON representation of the resource.</span></span>
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





