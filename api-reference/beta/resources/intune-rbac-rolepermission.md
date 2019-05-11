---
title: rolePermission 资源类型
description: 包含为每个角色确定允许和不允许的权限的一组 ResourceActions。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5ef360393e99b8c8a152596a2285cddd49d7e0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939026"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="7d2cb-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d2cb-103">rolePermission resource type</span></span>

> <span data-ttu-id="7d2cb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d2cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d2cb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d2cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d2cb-106">包含为每个角色确定允许和不允许的权限的一组 ResourceActions。</span><span class="sxs-lookup"><span data-stu-id="7d2cb-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="7d2cb-107">属性</span><span class="sxs-lookup"><span data-stu-id="7d2cb-107">Properties</span></span>
|<span data-ttu-id="7d2cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d2cb-108">Property</span></span>|<span data-ttu-id="7d2cb-109">类型</span><span class="sxs-lookup"><span data-stu-id="7d2cb-109">Type</span></span>|<span data-ttu-id="7d2cb-110">说明</span><span class="sxs-lookup"><span data-stu-id="7d2cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d2cb-111">actions</span><span class="sxs-lookup"><span data-stu-id="7d2cb-111">actions</span></span>|<span data-ttu-id="7d2cb-112">String collection</span><span class="sxs-lookup"><span data-stu-id="7d2cb-112">String collection</span></span>|<span data-ttu-id="7d2cb-113">允许的操作-已弃用</span><span class="sxs-lookup"><span data-stu-id="7d2cb-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="7d2cb-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="7d2cb-114">resourceActions</span></span>|<span data-ttu-id="7d2cb-115">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7d2cb-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="7d2cb-116">每个包含一组允许和不允许的权限的资源操作。</span><span class="sxs-lookup"><span data-stu-id="7d2cb-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d2cb-117">关系</span><span class="sxs-lookup"><span data-stu-id="7d2cb-117">Relationships</span></span>
<span data-ttu-id="7d2cb-118">无</span><span class="sxs-lookup"><span data-stu-id="7d2cb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d2cb-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d2cb-119">JSON Representation</span></span>
<span data-ttu-id="7d2cb-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d2cb-120">Here is a JSON representation of the resource.</span></span>
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




