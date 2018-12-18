---
title: rolePermission 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 0433c3f3a0ab3ef63fcd2a44776c083ddb5b91a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325674"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8cad2-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cad2-103">rolePermission resource type</span></span>

> <span data-ttu-id="8cad2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8cad2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cad2-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8cad2-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8cad2-106">属性</span><span class="sxs-lookup"><span data-stu-id="8cad2-106">Properties</span></span>
|<span data-ttu-id="8cad2-107">属性</span><span class="sxs-lookup"><span data-stu-id="8cad2-107">Property</span></span>|<span data-ttu-id="8cad2-108">类型</span><span class="sxs-lookup"><span data-stu-id="8cad2-108">Type</span></span>|<span data-ttu-id="8cad2-109">说明</span><span class="sxs-lookup"><span data-stu-id="8cad2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cad2-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8cad2-110">resourceActions</span></span>|<span data-ttu-id="8cad2-111">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8cad2-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8cad2-112">操作</span><span class="sxs-lookup"><span data-stu-id="8cad2-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cad2-113">关系</span><span class="sxs-lookup"><span data-stu-id="8cad2-113">Relationships</span></span>
<span data-ttu-id="8cad2-114">无</span><span class="sxs-lookup"><span data-stu-id="8cad2-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8cad2-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cad2-115">JSON Representation</span></span>
<span data-ttu-id="8cad2-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cad2-116">Here is a JSON representation of the resource.</span></span>
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



