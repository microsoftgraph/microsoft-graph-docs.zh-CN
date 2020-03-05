---
title: resourceAction 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae06b047fc93f09bd2b797a4eeaa296d232a0b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447960"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="e523f-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="e523f-103">resourceAction resource type</span></span>

<span data-ttu-id="e523f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e523f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e523f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e523f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e523f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e523f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e523f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e523f-107">Properties</span></span>
|<span data-ttu-id="e523f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e523f-108">Property</span></span>|<span data-ttu-id="e523f-109">类型</span><span class="sxs-lookup"><span data-stu-id="e523f-109">Type</span></span>|<span data-ttu-id="e523f-110">说明</span><span class="sxs-lookup"><span data-stu-id="e523f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e523f-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e523f-111">allowedResourceActions</span></span>|<span data-ttu-id="e523f-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="e523f-112">String collection</span></span>|<span data-ttu-id="e523f-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="e523f-113">Allowed Actions</span></span>|
|<span data-ttu-id="e523f-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e523f-114">notAllowedResourceActions</span></span>|<span data-ttu-id="e523f-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e523f-115">String collection</span></span>|<span data-ttu-id="e523f-116">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="e523f-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="e523f-117">关系</span><span class="sxs-lookup"><span data-stu-id="e523f-117">Relationships</span></span>
<span data-ttu-id="e523f-118">无</span><span class="sxs-lookup"><span data-stu-id="e523f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e523f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e523f-119">JSON Representation</span></span>
<span data-ttu-id="e523f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e523f-120">Here is a JSON representation of the resource.</span></span>
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




