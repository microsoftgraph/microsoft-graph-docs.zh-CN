---
title: rolePermission 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: c33af6af3bc06a53bd24ddf97576551a5eea6e9c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349103"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="89a31-103">rolePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="89a31-103">rolePermission resource type</span></span>

> <span data-ttu-id="89a31-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89a31-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89a31-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89a31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89a31-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89a31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89a31-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89a31-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="89a31-108">属性</span><span class="sxs-lookup"><span data-stu-id="89a31-108">Properties</span></span>
|<span data-ttu-id="89a31-109">属性</span><span class="sxs-lookup"><span data-stu-id="89a31-109">Property</span></span>|<span data-ttu-id="89a31-110">类型</span><span class="sxs-lookup"><span data-stu-id="89a31-110">Type</span></span>|<span data-ttu-id="89a31-111">说明</span><span class="sxs-lookup"><span data-stu-id="89a31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a31-112">actions</span><span class="sxs-lookup"><span data-stu-id="89a31-112">actions</span></span>|<span data-ttu-id="89a31-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89a31-113">String collection</span></span>|<span data-ttu-id="89a31-114">允许的操作</span><span class="sxs-lookup"><span data-stu-id="89a31-114">Allowed Actions</span></span>|
|<span data-ttu-id="89a31-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="89a31-115">resourceActions</span></span>|<span data-ttu-id="89a31-116">[resourceAction](../resources/intune-rbac-resourceaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89a31-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="89a31-117">操作</span><span class="sxs-lookup"><span data-stu-id="89a31-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="89a31-118">关系</span><span class="sxs-lookup"><span data-stu-id="89a31-118">Relationships</span></span>
<span data-ttu-id="89a31-119">无</span><span class="sxs-lookup"><span data-stu-id="89a31-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89a31-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89a31-120">JSON Representation</span></span>
<span data-ttu-id="89a31-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89a31-121">Here is a JSON representation of the resource.</span></span>
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





