---
title: rolePermission 资源类型
description: 包含为每个角色确定允许和不允许的权限的一组 ResourceActions。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2514200aec93288f1841190f0a0a5b3fdb556429
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725167"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="e8e19-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8e19-103">rolePermission resource type</span></span>

<span data-ttu-id="e8e19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8e19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8e19-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8e19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8e19-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8e19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8e19-107">包含为每个角色确定允许和不允许的权限的一组 ResourceActions。</span><span class="sxs-lookup"><span data-stu-id="e8e19-107">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="e8e19-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8e19-108">Properties</span></span>
|<span data-ttu-id="e8e19-109">属性</span><span class="sxs-lookup"><span data-stu-id="e8e19-109">Property</span></span>|<span data-ttu-id="e8e19-110">类型</span><span class="sxs-lookup"><span data-stu-id="e8e19-110">Type</span></span>|<span data-ttu-id="e8e19-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8e19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e19-112">actions</span><span class="sxs-lookup"><span data-stu-id="e8e19-112">actions</span></span>|<span data-ttu-id="e8e19-113">String collection</span><span class="sxs-lookup"><span data-stu-id="e8e19-113">String collection</span></span>|<span data-ttu-id="e8e19-114">允许的操作-已弃用</span><span class="sxs-lookup"><span data-stu-id="e8e19-114">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="e8e19-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="e8e19-115">resourceActions</span></span>|<span data-ttu-id="e8e19-116">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e8e19-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="e8e19-117">每个包含一组允许和不允许的权限的资源操作。</span><span class="sxs-lookup"><span data-stu-id="e8e19-117">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8e19-118">关系</span><span class="sxs-lookup"><span data-stu-id="e8e19-118">Relationships</span></span>
<span data-ttu-id="e8e19-119">无</span><span class="sxs-lookup"><span data-stu-id="e8e19-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8e19-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8e19-120">JSON Representation</span></span>
<span data-ttu-id="e8e19-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8e19-121">Here is a JSON representation of the resource.</span></span>
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





