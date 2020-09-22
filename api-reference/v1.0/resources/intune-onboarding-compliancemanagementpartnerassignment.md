---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9bdcfd0edcdf4e93b3bf11f8d30a3cef5cc9d60
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072968"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="cbd9b-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbd9b-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="cbd9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbd9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbd9b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbd9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbd9b-106">针对合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="cbd9b-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="cbd9b-107">属性</span><span class="sxs-lookup"><span data-stu-id="cbd9b-107">Properties</span></span>
|<span data-ttu-id="cbd9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbd9b-108">Property</span></span>|<span data-ttu-id="cbd9b-109">类型</span><span class="sxs-lookup"><span data-stu-id="cbd9b-109">Type</span></span>|<span data-ttu-id="cbd9b-110">说明</span><span class="sxs-lookup"><span data-stu-id="cbd9b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd9b-111">target</span><span class="sxs-lookup"><span data-stu-id="cbd9b-111">target</span></span>|[<span data-ttu-id="cbd9b-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cbd9b-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cbd9b-113">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="cbd9b-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbd9b-114">关系</span><span class="sxs-lookup"><span data-stu-id="cbd9b-114">Relationships</span></span>
<span data-ttu-id="cbd9b-115">无</span><span class="sxs-lookup"><span data-stu-id="cbd9b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbd9b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbd9b-116">JSON Representation</span></span>
<span data-ttu-id="cbd9b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbd9b-117">Here is a JSON representation of the resource.</span></span>
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





