---
title: deviceManagementPartnerAssignment 资源类型
description: 为设备管理合作伙伴设定目标的用户组
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 07a1dd94be6f73da420ba0cd3424030652eab2c5
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088201"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="8c6ce-103">deviceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c6ce-103">deviceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="8c6ce-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c6ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c6ce-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c6ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6ce-106">为设备管理合作伙伴设定目标的用户组</span><span class="sxs-lookup"><span data-stu-id="8c6ce-106">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="8c6ce-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c6ce-107">Properties</span></span>
|<span data-ttu-id="8c6ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c6ce-108">Property</span></span>|<span data-ttu-id="8c6ce-109">类型</span><span class="sxs-lookup"><span data-stu-id="8c6ce-109">Type</span></span>|<span data-ttu-id="8c6ce-110">描述</span><span class="sxs-lookup"><span data-stu-id="8c6ce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6ce-111">target</span><span class="sxs-lookup"><span data-stu-id="8c6ce-111">target</span></span>|[<span data-ttu-id="8c6ce-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8c6ce-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8c6ce-113">为要通过合作伙伴注册的设备设定的用户组。</span><span class="sxs-lookup"><span data-stu-id="8c6ce-113">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c6ce-114">关系</span><span class="sxs-lookup"><span data-stu-id="8c6ce-114">Relationships</span></span>
<span data-ttu-id="8c6ce-115">无</span><span class="sxs-lookup"><span data-stu-id="8c6ce-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c6ce-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c6ce-116">JSON Representation</span></span>
<span data-ttu-id="8c6ce-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c6ce-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



