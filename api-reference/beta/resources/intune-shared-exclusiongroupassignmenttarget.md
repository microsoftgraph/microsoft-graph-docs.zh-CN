---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ce17f38b3ab604a11710c64992a046f6d71a6659
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870705"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="00330-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="00330-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="00330-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00330-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00330-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00330-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00330-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00330-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00330-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="00330-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="00330-108">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="00330-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00330-109">属性</span><span class="sxs-lookup"><span data-stu-id="00330-109">Properties</span></span>
|<span data-ttu-id="00330-110">属性</span><span class="sxs-lookup"><span data-stu-id="00330-110">Property</span></span>|<span data-ttu-id="00330-111">类型</span><span class="sxs-lookup"><span data-stu-id="00330-111">Type</span></span>|<span data-ttu-id="00330-112">说明</span><span class="sxs-lookup"><span data-stu-id="00330-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00330-113">groupId</span><span class="sxs-lookup"><span data-stu-id="00330-113">groupId</span></span>|<span data-ttu-id="00330-114">String</span><span class="sxs-lookup"><span data-stu-id="00330-114">String</span></span>|<span data-ttu-id="00330-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="00330-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="00330-116">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="00330-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="00330-117">关系</span><span class="sxs-lookup"><span data-stu-id="00330-117">Relationships</span></span>
<span data-ttu-id="00330-118">无</span><span class="sxs-lookup"><span data-stu-id="00330-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00330-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00330-119">JSON Representation</span></span>
<span data-ttu-id="00330-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00330-120">Here is a JSON representation of the resource.</span></span>
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





