---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ddadab1682fa683dda815dab8c79182e8076e54c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473549"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="5110e-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="5110e-103">keyValuePair resource type</span></span>

<span data-ttu-id="5110e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5110e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5110e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5110e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5110e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5110e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5110e-107">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="5110e-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="5110e-108">属性</span><span class="sxs-lookup"><span data-stu-id="5110e-108">Properties</span></span>
|<span data-ttu-id="5110e-109">属性</span><span class="sxs-lookup"><span data-stu-id="5110e-109">Property</span></span>|<span data-ttu-id="5110e-110">类型</span><span class="sxs-lookup"><span data-stu-id="5110e-110">Type</span></span>|<span data-ttu-id="5110e-111">说明</span><span class="sxs-lookup"><span data-stu-id="5110e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5110e-112">name</span><span class="sxs-lookup"><span data-stu-id="5110e-112">name</span></span>|<span data-ttu-id="5110e-113">String</span><span class="sxs-lookup"><span data-stu-id="5110e-113">String</span></span>|<span data-ttu-id="5110e-114">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="5110e-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="5110e-115">value</span><span class="sxs-lookup"><span data-stu-id="5110e-115">value</span></span>|<span data-ttu-id="5110e-116">String</span><span class="sxs-lookup"><span data-stu-id="5110e-116">String</span></span>|<span data-ttu-id="5110e-117">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="5110e-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="5110e-118">关系</span><span class="sxs-lookup"><span data-stu-id="5110e-118">Relationships</span></span>
<span data-ttu-id="5110e-119">无</span><span class="sxs-lookup"><span data-stu-id="5110e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5110e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5110e-120">JSON Representation</span></span>
<span data-ttu-id="5110e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5110e-121">Here is a JSON representation of the resource.</span></span>
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



