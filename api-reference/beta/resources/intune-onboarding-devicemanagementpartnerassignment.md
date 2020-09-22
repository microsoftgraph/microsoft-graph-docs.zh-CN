---
title: deviceManagementPartnerAssignment 资源类型
description: 为设备管理合作伙伴设定目标的用户组
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdfa45e87091a1a98a7cbdb29b310e5fce4daea5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029510"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="bd9d3-103">deviceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd9d3-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="bd9d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd9d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd9d3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd9d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd9d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd9d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd9d3-107">为设备管理合作伙伴设定目标的用户组</span><span class="sxs-lookup"><span data-stu-id="bd9d3-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="bd9d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd9d3-108">Properties</span></span>
|<span data-ttu-id="bd9d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="bd9d3-109">Property</span></span>|<span data-ttu-id="bd9d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="bd9d3-110">Type</span></span>|<span data-ttu-id="bd9d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="bd9d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd9d3-112">target</span><span class="sxs-lookup"><span data-stu-id="bd9d3-112">target</span></span>|[<span data-ttu-id="bd9d3-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bd9d3-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bd9d3-114">为要通过合作伙伴注册的设备设定的用户组。</span><span class="sxs-lookup"><span data-stu-id="bd9d3-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd9d3-115">关系</span><span class="sxs-lookup"><span data-stu-id="bd9d3-115">Relationships</span></span>
<span data-ttu-id="bd9d3-116">无</span><span class="sxs-lookup"><span data-stu-id="bd9d3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd9d3-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd9d3-117">JSON Representation</span></span>
<span data-ttu-id="bd9d3-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd9d3-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```






