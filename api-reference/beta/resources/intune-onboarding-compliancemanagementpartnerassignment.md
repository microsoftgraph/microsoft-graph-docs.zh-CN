---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b557cde710ac0d2a4820c71b7e595ad49e6f026
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697306"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="e662a-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e662a-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="e662a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e662a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e662a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e662a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e662a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e662a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e662a-107">针对合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="e662a-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="e662a-108">属性</span><span class="sxs-lookup"><span data-stu-id="e662a-108">Properties</span></span>
|<span data-ttu-id="e662a-109">属性</span><span class="sxs-lookup"><span data-stu-id="e662a-109">Property</span></span>|<span data-ttu-id="e662a-110">类型</span><span class="sxs-lookup"><span data-stu-id="e662a-110">Type</span></span>|<span data-ttu-id="e662a-111">说明</span><span class="sxs-lookup"><span data-stu-id="e662a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e662a-112">target</span><span class="sxs-lookup"><span data-stu-id="e662a-112">target</span></span>|[<span data-ttu-id="e662a-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e662a-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e662a-114">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="e662a-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e662a-115">关系</span><span class="sxs-lookup"><span data-stu-id="e662a-115">Relationships</span></span>
<span data-ttu-id="e662a-116">无</span><span class="sxs-lookup"><span data-stu-id="e662a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e662a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e662a-117">JSON Representation</span></span>
<span data-ttu-id="e662a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e662a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```





