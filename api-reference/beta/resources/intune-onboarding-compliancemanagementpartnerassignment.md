---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 833a2dee09caae20b9a58fb5c82d9de06ce5cf33
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418957"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="7c4cc-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c4cc-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="7c4cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c4cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c4cc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c4cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c4cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c4cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c4cc-107">针对合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="7c4cc-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="7c4cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c4cc-108">Properties</span></span>
|<span data-ttu-id="7c4cc-109">属性</span><span class="sxs-lookup"><span data-stu-id="7c4cc-109">Property</span></span>|<span data-ttu-id="7c4cc-110">类型</span><span class="sxs-lookup"><span data-stu-id="7c4cc-110">Type</span></span>|<span data-ttu-id="7c4cc-111">说明</span><span class="sxs-lookup"><span data-stu-id="7c4cc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c4cc-112">target</span><span class="sxs-lookup"><span data-stu-id="7c4cc-112">target</span></span>|[<span data-ttu-id="7c4cc-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c4cc-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7c4cc-114">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="7c4cc-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c4cc-115">关系</span><span class="sxs-lookup"><span data-stu-id="7c4cc-115">Relationships</span></span>
<span data-ttu-id="7c4cc-116">无</span><span class="sxs-lookup"><span data-stu-id="7c4cc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c4cc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c4cc-117">JSON Representation</span></span>
<span data-ttu-id="7c4cc-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c4cc-118">Here is a JSON representation of the resource.</span></span>
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



