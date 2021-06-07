---
title: complianceManagementPartnerAssignment 资源类型
description: 合规性管理合作伙伴的用户组目标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 638a50d7c8a6f1723c841c21f06d8cb44ac65460
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755649"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="de700-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="de700-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="de700-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de700-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de700-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de700-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de700-106">合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="de700-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="de700-107">属性</span><span class="sxs-lookup"><span data-stu-id="de700-107">Properties</span></span>
|<span data-ttu-id="de700-108">属性</span><span class="sxs-lookup"><span data-stu-id="de700-108">Property</span></span>|<span data-ttu-id="de700-109">类型</span><span class="sxs-lookup"><span data-stu-id="de700-109">Type</span></span>|<span data-ttu-id="de700-110">说明</span><span class="sxs-lookup"><span data-stu-id="de700-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de700-111">target</span><span class="sxs-lookup"><span data-stu-id="de700-111">target</span></span>|[<span data-ttu-id="de700-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de700-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de700-113">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="de700-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de700-114">关系</span><span class="sxs-lookup"><span data-stu-id="de700-114">Relationships</span></span>
<span data-ttu-id="de700-115">无</span><span class="sxs-lookup"><span data-stu-id="de700-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de700-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de700-116">JSON Representation</span></span>
<span data-ttu-id="de700-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de700-117">Here is a JSON representation of the resource.</span></span>
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
    "collectionId": "String"
  }
}
```




