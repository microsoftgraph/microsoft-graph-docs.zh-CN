---
title: deviceManagementPartnerAssignment 资源类型
description: 设备管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0cda49b654313ec4d69e810033ae681b8ac2645
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157538"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="66246-103">deviceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="66246-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="66246-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66246-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66246-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66246-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66246-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66246-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66246-107">设备管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="66246-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="66246-108">属性</span><span class="sxs-lookup"><span data-stu-id="66246-108">Properties</span></span>
|<span data-ttu-id="66246-109">属性</span><span class="sxs-lookup"><span data-stu-id="66246-109">Property</span></span>|<span data-ttu-id="66246-110">类型</span><span class="sxs-lookup"><span data-stu-id="66246-110">Type</span></span>|<span data-ttu-id="66246-111">说明</span><span class="sxs-lookup"><span data-stu-id="66246-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66246-112">target</span><span class="sxs-lookup"><span data-stu-id="66246-112">target</span></span>|[<span data-ttu-id="66246-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="66246-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="66246-114">面向要通过合作伙伴注册的设备的用户组。</span><span class="sxs-lookup"><span data-stu-id="66246-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66246-115">关系</span><span class="sxs-lookup"><span data-stu-id="66246-115">Relationships</span></span>
<span data-ttu-id="66246-116">无</span><span class="sxs-lookup"><span data-stu-id="66246-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66246-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66246-117">JSON Representation</span></span>
<span data-ttu-id="66246-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66246-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




