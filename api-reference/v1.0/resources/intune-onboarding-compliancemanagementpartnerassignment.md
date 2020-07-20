---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cf246cd1f7fad0d168165f72a3861005e8cefbe
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744119"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="cc2af-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc2af-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="cc2af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc2af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc2af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc2af-106">针对合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="cc2af-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="cc2af-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc2af-107">Properties</span></span>
|<span data-ttu-id="cc2af-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc2af-108">Property</span></span>|<span data-ttu-id="cc2af-109">类型</span><span class="sxs-lookup"><span data-stu-id="cc2af-109">Type</span></span>|<span data-ttu-id="cc2af-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc2af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc2af-111">target</span><span class="sxs-lookup"><span data-stu-id="cc2af-111">target</span></span>|[<span data-ttu-id="cc2af-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cc2af-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cc2af-113">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="cc2af-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc2af-114">关系</span><span class="sxs-lookup"><span data-stu-id="cc2af-114">Relationships</span></span>
<span data-ttu-id="cc2af-115">无</span><span class="sxs-lookup"><span data-stu-id="cc2af-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc2af-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc2af-116">JSON Representation</span></span>
<span data-ttu-id="cc2af-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc2af-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



