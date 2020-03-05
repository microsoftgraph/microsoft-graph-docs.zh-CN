---
title: rolePermission 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3a01bf7c6f607c7340cff8ea5075a24fb879ddb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447925"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="ffbd7-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffbd7-103">rolePermission resource type</span></span>

<span data-ttu-id="ffbd7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ffbd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffbd7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffbd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffbd7-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ffbd7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ffbd7-107">属性</span><span class="sxs-lookup"><span data-stu-id="ffbd7-107">Properties</span></span>
|<span data-ttu-id="ffbd7-108">属性</span><span class="sxs-lookup"><span data-stu-id="ffbd7-108">Property</span></span>|<span data-ttu-id="ffbd7-109">类型</span><span class="sxs-lookup"><span data-stu-id="ffbd7-109">Type</span></span>|<span data-ttu-id="ffbd7-110">说明</span><span class="sxs-lookup"><span data-stu-id="ffbd7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffbd7-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="ffbd7-111">resourceActions</span></span>|<span data-ttu-id="ffbd7-112">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ffbd7-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="ffbd7-113">操作</span><span class="sxs-lookup"><span data-stu-id="ffbd7-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffbd7-114">关系</span><span class="sxs-lookup"><span data-stu-id="ffbd7-114">Relationships</span></span>
<span data-ttu-id="ffbd7-115">无</span><span class="sxs-lookup"><span data-stu-id="ffbd7-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffbd7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffbd7-116">JSON Representation</span></span>
<span data-ttu-id="ffbd7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffbd7-117">Here is a JSON representation of the resource.</span></span>
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




