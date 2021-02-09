---
title: complianceManagementPartnerAssignment 资源类型
description: 合规性管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46e4e6a5e073e3087267329880cf0f36bb79c4a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161437"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="2d681-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d681-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="2d681-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d681-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d681-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d681-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d681-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d681-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d681-107">合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="2d681-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="2d681-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d681-108">Properties</span></span>
|<span data-ttu-id="2d681-109">属性</span><span class="sxs-lookup"><span data-stu-id="2d681-109">Property</span></span>|<span data-ttu-id="2d681-110">类型</span><span class="sxs-lookup"><span data-stu-id="2d681-110">Type</span></span>|<span data-ttu-id="2d681-111">说明</span><span class="sxs-lookup"><span data-stu-id="2d681-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d681-112">target</span><span class="sxs-lookup"><span data-stu-id="2d681-112">target</span></span>|[<span data-ttu-id="2d681-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2d681-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2d681-114">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="2d681-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d681-115">关系</span><span class="sxs-lookup"><span data-stu-id="2d681-115">Relationships</span></span>
<span data-ttu-id="2d681-116">无</span><span class="sxs-lookup"><span data-stu-id="2d681-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d681-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d681-117">JSON Representation</span></span>
<span data-ttu-id="2d681-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d681-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




