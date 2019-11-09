---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 51dc2a8f4861f160db6a3775526ec7fdd4e85ea7
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088215"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="8ae16-103">complianceManagementPartnerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ae16-103">complianceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="8ae16-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ae16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ae16-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ae16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae16-106">针对合规性管理合作伙伴的用户组目标</span><span class="sxs-lookup"><span data-stu-id="8ae16-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="8ae16-107">属性</span><span class="sxs-lookup"><span data-stu-id="8ae16-107">Properties</span></span>
|<span data-ttu-id="8ae16-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ae16-108">Property</span></span>|<span data-ttu-id="8ae16-109">类型</span><span class="sxs-lookup"><span data-stu-id="8ae16-109">Type</span></span>|<span data-ttu-id="8ae16-110">描述</span><span class="sxs-lookup"><span data-stu-id="8ae16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae16-111">target</span><span class="sxs-lookup"><span data-stu-id="8ae16-111">target</span></span>|[<span data-ttu-id="8ae16-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8ae16-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8ae16-113">组分配目标。</span><span class="sxs-lookup"><span data-stu-id="8ae16-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ae16-114">关系</span><span class="sxs-lookup"><span data-stu-id="8ae16-114">Relationships</span></span>
<span data-ttu-id="8ae16-115">无</span><span class="sxs-lookup"><span data-stu-id="8ae16-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ae16-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ae16-116">JSON Representation</span></span>
<span data-ttu-id="8ae16-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ae16-117">Here is a JSON representation of the resource.</span></span>
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



