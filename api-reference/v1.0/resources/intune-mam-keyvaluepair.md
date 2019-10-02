---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2849e6adfc0b43b9091764cd2706d5c572826774
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356434"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="61fb7-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="61fb7-103">keyValuePair resource type</span></span>

> <span data-ttu-id="61fb7-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61fb7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61fb7-105">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="61fb7-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="61fb7-106">属性</span><span class="sxs-lookup"><span data-stu-id="61fb7-106">Properties</span></span>
|<span data-ttu-id="61fb7-107">属性</span><span class="sxs-lookup"><span data-stu-id="61fb7-107">Property</span></span>|<span data-ttu-id="61fb7-108">类型</span><span class="sxs-lookup"><span data-stu-id="61fb7-108">Type</span></span>|<span data-ttu-id="61fb7-109">说明</span><span class="sxs-lookup"><span data-stu-id="61fb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61fb7-110">name</span><span class="sxs-lookup"><span data-stu-id="61fb7-110">name</span></span>|<span data-ttu-id="61fb7-111">String</span><span class="sxs-lookup"><span data-stu-id="61fb7-111">String</span></span>|<span data-ttu-id="61fb7-112">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="61fb7-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="61fb7-113">value</span><span class="sxs-lookup"><span data-stu-id="61fb7-113">value</span></span>|<span data-ttu-id="61fb7-114">String</span><span class="sxs-lookup"><span data-stu-id="61fb7-114">String</span></span>|<span data-ttu-id="61fb7-115">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="61fb7-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="61fb7-116">关系</span><span class="sxs-lookup"><span data-stu-id="61fb7-116">Relationships</span></span>
<span data-ttu-id="61fb7-117">无</span><span class="sxs-lookup"><span data-stu-id="61fb7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61fb7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61fb7-118">JSON Representation</span></span>
<span data-ttu-id="61fb7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61fb7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```




