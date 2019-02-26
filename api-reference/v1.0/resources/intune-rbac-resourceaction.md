---
title: resourceAction 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262179"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="87858-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="87858-103">resourceAction resource type</span></span>

> <span data-ttu-id="87858-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87858-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87858-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87858-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="87858-106">属性</span><span class="sxs-lookup"><span data-stu-id="87858-106">Properties</span></span>
|<span data-ttu-id="87858-107">属性</span><span class="sxs-lookup"><span data-stu-id="87858-107">Property</span></span>|<span data-ttu-id="87858-108">类型</span><span class="sxs-lookup"><span data-stu-id="87858-108">Type</span></span>|<span data-ttu-id="87858-109">说明</span><span class="sxs-lookup"><span data-stu-id="87858-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87858-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="87858-110">allowedResourceActions</span></span>|<span data-ttu-id="87858-111">String collection</span><span class="sxs-lookup"><span data-stu-id="87858-111">String collection</span></span>|<span data-ttu-id="87858-112">允许的操作</span><span class="sxs-lookup"><span data-stu-id="87858-112">Allowed Actions</span></span>|
|<span data-ttu-id="87858-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="87858-113">notAllowedResourceActions</span></span>|<span data-ttu-id="87858-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="87858-114">String collection</span></span>|<span data-ttu-id="87858-115">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="87858-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="87858-116">关系</span><span class="sxs-lookup"><span data-stu-id="87858-116">Relationships</span></span>
<span data-ttu-id="87858-117">无</span><span class="sxs-lookup"><span data-stu-id="87858-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87858-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87858-118">JSON Representation</span></span>
<span data-ttu-id="87858-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87858-119">Here is a JSON representation of the resource.</span></span>
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



