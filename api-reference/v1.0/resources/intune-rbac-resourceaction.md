---
title: resourceAction 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ea0c947a87135f874755f49d0847a3c2a08fae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037154"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="fdc08-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdc08-103">resourceAction resource type</span></span>

> <span data-ttu-id="fdc08-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fdc08-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc08-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fdc08-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fdc08-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdc08-106">Properties</span></span>
|<span data-ttu-id="fdc08-107">属性</span><span class="sxs-lookup"><span data-stu-id="fdc08-107">Property</span></span>|<span data-ttu-id="fdc08-108">类型</span><span class="sxs-lookup"><span data-stu-id="fdc08-108">Type</span></span>|<span data-ttu-id="fdc08-109">说明</span><span class="sxs-lookup"><span data-stu-id="fdc08-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc08-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="fdc08-110">allowedResourceActions</span></span>|<span data-ttu-id="fdc08-111">String collection</span><span class="sxs-lookup"><span data-stu-id="fdc08-111">String collection</span></span>|<span data-ttu-id="fdc08-112">允许的操作</span><span class="sxs-lookup"><span data-stu-id="fdc08-112">Allowed Actions</span></span>|
|<span data-ttu-id="fdc08-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="fdc08-113">notAllowedResourceActions</span></span>|<span data-ttu-id="fdc08-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="fdc08-114">String collection</span></span>|<span data-ttu-id="fdc08-115">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="fdc08-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdc08-116">关系</span><span class="sxs-lookup"><span data-stu-id="fdc08-116">Relationships</span></span>
<span data-ttu-id="fdc08-117">无</span><span class="sxs-lookup"><span data-stu-id="fdc08-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdc08-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdc08-118">JSON Representation</span></span>
<span data-ttu-id="fdc08-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdc08-119">Here is a JSON representation of the resource.</span></span>
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



