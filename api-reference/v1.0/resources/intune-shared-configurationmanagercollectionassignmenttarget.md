---
title: configurationManagerCollectionAssignmentTarget 资源类型
description: 表示对 Configuration Manager 集合的分配。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28aa1e4e7fbb0d65a74f9a7b84bc48df19f3201c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751808"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="9d2e1-103">configurationManagerCollectionAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d2e1-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="9d2e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d2e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d2e1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d2e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d2e1-106">表示对 Configuration Manager 集合的分配。</span><span class="sxs-lookup"><span data-stu-id="9d2e1-106">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="9d2e1-107">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9d2e1-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9d2e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d2e1-108">Properties</span></span>
|<span data-ttu-id="9d2e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d2e1-109">Property</span></span>|<span data-ttu-id="9d2e1-110">类型</span><span class="sxs-lookup"><span data-stu-id="9d2e1-110">Type</span></span>|<span data-ttu-id="9d2e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d2e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d2e1-112">collectionId</span><span class="sxs-lookup"><span data-stu-id="9d2e1-112">collectionId</span></span>|<span data-ttu-id="9d2e1-113">String</span><span class="sxs-lookup"><span data-stu-id="9d2e1-113">String</span></span>|<span data-ttu-id="9d2e1-114">作为工作分配目标的集合 ID。</span><span class="sxs-lookup"><span data-stu-id="9d2e1-114">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d2e1-115">关系</span><span class="sxs-lookup"><span data-stu-id="9d2e1-115">Relationships</span></span>
<span data-ttu-id="9d2e1-116">无</span><span class="sxs-lookup"><span data-stu-id="9d2e1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d2e1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d2e1-117">JSON Representation</span></span>
<span data-ttu-id="9d2e1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d2e1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "collectionId": "String"
}
```




