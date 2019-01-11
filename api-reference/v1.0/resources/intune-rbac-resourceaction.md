---
title: resourceAction 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a0ce30dc6e9607aa1531e7421af6b7a5500939
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870728"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="bb0c4-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb0c4-103">resourceAction resource type</span></span>

> <span data-ttu-id="bb0c4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb0c4-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bb0c4-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bb0c4-106">属性</span><span class="sxs-lookup"><span data-stu-id="bb0c4-106">Properties</span></span>
|<span data-ttu-id="bb0c4-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb0c4-107">Property</span></span>|<span data-ttu-id="bb0c4-108">类型</span><span class="sxs-lookup"><span data-stu-id="bb0c4-108">Type</span></span>|<span data-ttu-id="bb0c4-109">说明</span><span class="sxs-lookup"><span data-stu-id="bb0c4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0c4-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="bb0c4-110">allowedResourceActions</span></span>|<span data-ttu-id="bb0c4-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="bb0c4-111">String collection</span></span>|<span data-ttu-id="bb0c4-112">允许的操作</span><span class="sxs-lookup"><span data-stu-id="bb0c4-112">Allowed Actions</span></span>|
|<span data-ttu-id="bb0c4-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="bb0c4-113">notAllowedResourceActions</span></span>|<span data-ttu-id="bb0c4-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="bb0c4-114">String collection</span></span>|<span data-ttu-id="bb0c4-115">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="bb0c4-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb0c4-116">关系</span><span class="sxs-lookup"><span data-stu-id="bb0c4-116">Relationships</span></span>
<span data-ttu-id="bb0c4-117">无</span><span class="sxs-lookup"><span data-stu-id="bb0c4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb0c4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb0c4-118">JSON Representation</span></span>
<span data-ttu-id="bb0c4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



