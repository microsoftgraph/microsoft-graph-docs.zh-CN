---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7218fc69564ea08a7302cfb0af7856360cd9a330
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809042"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="40f42-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="40f42-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="40f42-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="40f42-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40f42-105">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="40f42-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="40f42-106">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="40f42-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="40f42-107">属性</span><span class="sxs-lookup"><span data-stu-id="40f42-107">Properties</span></span>
|<span data-ttu-id="40f42-108">属性</span><span class="sxs-lookup"><span data-stu-id="40f42-108">Property</span></span>|<span data-ttu-id="40f42-109">类型</span><span class="sxs-lookup"><span data-stu-id="40f42-109">Type</span></span>|<span data-ttu-id="40f42-110">说明</span><span class="sxs-lookup"><span data-stu-id="40f42-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40f42-111">groupId</span><span class="sxs-lookup"><span data-stu-id="40f42-111">groupId</span></span>|<span data-ttu-id="40f42-112">String</span><span class="sxs-lookup"><span data-stu-id="40f42-112">String</span></span>|<span data-ttu-id="40f42-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="40f42-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40f42-114">关系</span><span class="sxs-lookup"><span data-stu-id="40f42-114">Relationships</span></span>
<span data-ttu-id="40f42-115">无</span><span class="sxs-lookup"><span data-stu-id="40f42-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40f42-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40f42-116">JSON Representation</span></span>
<span data-ttu-id="40f42-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40f42-117">Here is a JSON representation of the resource.</span></span>
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



