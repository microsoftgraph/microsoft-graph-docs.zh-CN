---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: tfitzmac
ms.openlocfilehash: 5371554d069237dc6bc017c29574423b415f4f33
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323133"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="d6208-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6208-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d6208-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6208-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6208-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6208-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6208-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d6208-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6208-107">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="d6208-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="d6208-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d6208-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6208-109">属性</span><span class="sxs-lookup"><span data-stu-id="d6208-109">Properties</span></span>
|<span data-ttu-id="d6208-110">属性</span><span class="sxs-lookup"><span data-stu-id="d6208-110">Property</span></span>|<span data-ttu-id="d6208-111">类型</span><span class="sxs-lookup"><span data-stu-id="d6208-111">Type</span></span>|<span data-ttu-id="d6208-112">说明</span><span class="sxs-lookup"><span data-stu-id="d6208-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6208-113">groupId</span><span class="sxs-lookup"><span data-stu-id="d6208-113">groupId</span></span>|<span data-ttu-id="d6208-114">String</span><span class="sxs-lookup"><span data-stu-id="d6208-114">String</span></span>|<span data-ttu-id="d6208-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="d6208-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6208-116">关系</span><span class="sxs-lookup"><span data-stu-id="d6208-116">Relationships</span></span>
<span data-ttu-id="d6208-117">无</span><span class="sxs-lookup"><span data-stu-id="d6208-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6208-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6208-118">JSON Representation</span></span>
<span data-ttu-id="d6208-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6208-119">Here is a JSON representation of the resource.</span></span>
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





