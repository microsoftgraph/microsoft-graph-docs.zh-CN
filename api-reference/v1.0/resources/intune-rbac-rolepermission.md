---
title: rolePermission 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90de4e78bbc831ebb9eb7bf5ee65c26434fc06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554112"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="495ee-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="495ee-103">rolePermission resource type</span></span>

> <span data-ttu-id="495ee-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="495ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="495ee-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="495ee-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="495ee-106">属性</span><span class="sxs-lookup"><span data-stu-id="495ee-106">Properties</span></span>
|<span data-ttu-id="495ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="495ee-107">Property</span></span>|<span data-ttu-id="495ee-108">类型</span><span class="sxs-lookup"><span data-stu-id="495ee-108">Type</span></span>|<span data-ttu-id="495ee-109">说明</span><span class="sxs-lookup"><span data-stu-id="495ee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="495ee-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="495ee-110">resourceActions</span></span>|<span data-ttu-id="495ee-111">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="495ee-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="495ee-112">操作</span><span class="sxs-lookup"><span data-stu-id="495ee-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="495ee-113">关系</span><span class="sxs-lookup"><span data-stu-id="495ee-113">Relationships</span></span>
<span data-ttu-id="495ee-114">无</span><span class="sxs-lookup"><span data-stu-id="495ee-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="495ee-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="495ee-115">JSON Representation</span></span>
<span data-ttu-id="495ee-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="495ee-116">Here is a JSON representation of the resource.</span></span>
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



