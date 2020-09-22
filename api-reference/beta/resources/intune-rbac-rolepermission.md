---
title: rolePermission 资源类型
description: 包含为每个角色确定允许和不允许的权限的一组 ResourceActions。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8627639d0eabed4392ed3d6763731dc4b65113c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039487"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="2fec7-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fec7-103">rolePermission resource type</span></span>

<span data-ttu-id="2fec7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fec7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fec7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2fec7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fec7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2fec7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fec7-107">包含为每个角色确定允许和不允许的权限的一组 ResourceActions。</span><span class="sxs-lookup"><span data-stu-id="2fec7-107">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="2fec7-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fec7-108">Properties</span></span>
|<span data-ttu-id="2fec7-109">属性</span><span class="sxs-lookup"><span data-stu-id="2fec7-109">Property</span></span>|<span data-ttu-id="2fec7-110">类型</span><span class="sxs-lookup"><span data-stu-id="2fec7-110">Type</span></span>|<span data-ttu-id="2fec7-111">说明</span><span class="sxs-lookup"><span data-stu-id="2fec7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fec7-112">actions</span><span class="sxs-lookup"><span data-stu-id="2fec7-112">actions</span></span>|<span data-ttu-id="2fec7-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="2fec7-113">String collection</span></span>|<span data-ttu-id="2fec7-114">允许的操作-已弃用</span><span class="sxs-lookup"><span data-stu-id="2fec7-114">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="2fec7-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2fec7-115">resourceActions</span></span>|<span data-ttu-id="2fec7-116">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fec7-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="2fec7-117">每个包含一组允许和不允许的权限的资源操作。</span><span class="sxs-lookup"><span data-stu-id="2fec7-117">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fec7-118">关系</span><span class="sxs-lookup"><span data-stu-id="2fec7-118">Relationships</span></span>
<span data-ttu-id="2fec7-119">无</span><span class="sxs-lookup"><span data-stu-id="2fec7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fec7-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fec7-120">JSON Representation</span></span>
<span data-ttu-id="2fec7-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fec7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
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






