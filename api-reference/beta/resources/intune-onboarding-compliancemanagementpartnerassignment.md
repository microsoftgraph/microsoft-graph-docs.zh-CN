---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83652eb419566836c349fd2f12160516710c710b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779798"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="f9572-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9572-103">complianceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="f9572-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9572-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9572-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9572-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9572-106">针对合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="f9572-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="f9572-107">属性</span><span class="sxs-lookup"><span data-stu-id="f9572-107">Properties</span></span>
|<span data-ttu-id="f9572-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9572-108">Property</span></span>|<span data-ttu-id="f9572-109">类型</span><span class="sxs-lookup"><span data-stu-id="f9572-109">Type</span></span>|<span data-ttu-id="f9572-110">说明</span><span class="sxs-lookup"><span data-stu-id="f9572-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9572-111">target</span><span class="sxs-lookup"><span data-stu-id="f9572-111">target</span></span>|[<span data-ttu-id="f9572-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f9572-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f9572-113">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="f9572-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9572-114">关系</span><span class="sxs-lookup"><span data-stu-id="f9572-114">Relationships</span></span>
<span data-ttu-id="f9572-115">无</span><span class="sxs-lookup"><span data-stu-id="f9572-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9572-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9572-116">JSON Representation</span></span>
<span data-ttu-id="f9572-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9572-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



