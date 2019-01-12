---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96aec1b72233cfe7d553b8f17feb9af382d89cde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971674"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="92a63-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="92a63-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="92a63-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="92a63-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92a63-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="92a63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92a63-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="92a63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92a63-107">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="92a63-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="92a63-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="92a63-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92a63-109">属性</span><span class="sxs-lookup"><span data-stu-id="92a63-109">Properties</span></span>
|<span data-ttu-id="92a63-110">属性</span><span class="sxs-lookup"><span data-stu-id="92a63-110">Property</span></span>|<span data-ttu-id="92a63-111">类型</span><span class="sxs-lookup"><span data-stu-id="92a63-111">Type</span></span>|<span data-ttu-id="92a63-112">说明</span><span class="sxs-lookup"><span data-stu-id="92a63-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a63-113">groupId</span><span class="sxs-lookup"><span data-stu-id="92a63-113">groupId</span></span>|<span data-ttu-id="92a63-114">String</span><span class="sxs-lookup"><span data-stu-id="92a63-114">String</span></span>|<span data-ttu-id="92a63-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="92a63-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92a63-116">关系</span><span class="sxs-lookup"><span data-stu-id="92a63-116">Relationships</span></span>
<span data-ttu-id="92a63-117">无</span><span class="sxs-lookup"><span data-stu-id="92a63-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92a63-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92a63-118">JSON Representation</span></span>
<span data-ttu-id="92a63-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92a63-119">Here is a JSON representation of the resource.</span></span>
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





