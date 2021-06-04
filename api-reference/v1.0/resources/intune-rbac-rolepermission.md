---
title: rolePermission 资源类型
description: 包含一组 ResourceActions，用于确定每个角色的允许和不允许的权限。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7598e7f7a54910d706ec95741234a38a9a9ba422
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752747"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="2d290-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d290-103">rolePermission resource type</span></span>

<span data-ttu-id="2d290-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d290-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d290-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d290-106">包含一组 ResourceActions，用于确定每个角色的允许和不允许的权限。</span><span class="sxs-lookup"><span data-stu-id="2d290-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="2d290-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d290-107">Properties</span></span>
|<span data-ttu-id="2d290-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d290-108">Property</span></span>|<span data-ttu-id="2d290-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d290-109">Type</span></span>|<span data-ttu-id="2d290-110">Description</span><span class="sxs-lookup"><span data-stu-id="2d290-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d290-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2d290-111">resourceActions</span></span>|<span data-ttu-id="2d290-112">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d290-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="2d290-113">资源操作每个包含一组允许和不允许的权限。</span><span class="sxs-lookup"><span data-stu-id="2d290-113">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d290-114">关系</span><span class="sxs-lookup"><span data-stu-id="2d290-114">Relationships</span></span>
<span data-ttu-id="2d290-115">无</span><span class="sxs-lookup"><span data-stu-id="2d290-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d290-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d290-116">JSON Representation</span></span>
<span data-ttu-id="2d290-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d290-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```




