---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e2928817a4d8bf287c3a941ddea80e7a3c4e19fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951717"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="8a238-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a238-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="8a238-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8a238-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a238-105">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="8a238-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="8a238-106">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="8a238-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a238-107">属性</span><span class="sxs-lookup"><span data-stu-id="8a238-107">Properties</span></span>
|<span data-ttu-id="8a238-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a238-108">Property</span></span>|<span data-ttu-id="8a238-109">类型</span><span class="sxs-lookup"><span data-stu-id="8a238-109">Type</span></span>|<span data-ttu-id="8a238-110">说明</span><span class="sxs-lookup"><span data-stu-id="8a238-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a238-111">groupId</span><span class="sxs-lookup"><span data-stu-id="8a238-111">groupId</span></span>|<span data-ttu-id="8a238-112">String</span><span class="sxs-lookup"><span data-stu-id="8a238-112">String</span></span>|<span data-ttu-id="8a238-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="8a238-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a238-114">关系</span><span class="sxs-lookup"><span data-stu-id="8a238-114">Relationships</span></span>
<span data-ttu-id="8a238-115">无</span><span class="sxs-lookup"><span data-stu-id="8a238-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a238-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a238-116">JSON Representation</span></span>
<span data-ttu-id="8a238-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a238-117">Here is a JSON representation of the resource.</span></span>
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



