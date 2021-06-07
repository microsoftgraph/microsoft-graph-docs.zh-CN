---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3deb1d366396bf97133b4984bda2b67609fcdee6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751662"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="a9b3b-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9b3b-103">keyValuePair resource type</span></span>

<span data-ttu-id="a9b3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9b3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9b3b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9b3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b3b-106">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="a9b3b-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="a9b3b-107">属性</span><span class="sxs-lookup"><span data-stu-id="a9b3b-107">Properties</span></span>
|<span data-ttu-id="a9b3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9b3b-108">Property</span></span>|<span data-ttu-id="a9b3b-109">类型</span><span class="sxs-lookup"><span data-stu-id="a9b3b-109">Type</span></span>|<span data-ttu-id="a9b3b-110">Description</span><span class="sxs-lookup"><span data-stu-id="a9b3b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b3b-111">name</span><span class="sxs-lookup"><span data-stu-id="a9b3b-111">name</span></span>|<span data-ttu-id="a9b3b-112">String</span><span class="sxs-lookup"><span data-stu-id="a9b3b-112">String</span></span>|<span data-ttu-id="a9b3b-113">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="a9b3b-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="a9b3b-114">value</span><span class="sxs-lookup"><span data-stu-id="a9b3b-114">value</span></span>|<span data-ttu-id="a9b3b-115">String</span><span class="sxs-lookup"><span data-stu-id="a9b3b-115">String</span></span>|<span data-ttu-id="a9b3b-116">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="a9b3b-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9b3b-117">关系</span><span class="sxs-lookup"><span data-stu-id="a9b3b-117">Relationships</span></span>
<span data-ttu-id="a9b3b-118">无</span><span class="sxs-lookup"><span data-stu-id="a9b3b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9b3b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9b3b-119">JSON Representation</span></span>
<span data-ttu-id="a9b3b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9b3b-120">Here is a JSON representation of the resource.</span></span>
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




