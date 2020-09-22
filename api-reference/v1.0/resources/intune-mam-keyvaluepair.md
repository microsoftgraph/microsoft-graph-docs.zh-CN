---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb3e5e47b6c4594fa366101e83cc1453400db00c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984388"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="4e5f6-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e5f6-103">keyValuePair resource type</span></span>

<span data-ttu-id="4e5f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e5f6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e5f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e5f6-106">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="4e5f6-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="4e5f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e5f6-107">Properties</span></span>
|<span data-ttu-id="4e5f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e5f6-108">Property</span></span>|<span data-ttu-id="4e5f6-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e5f6-109">Type</span></span>|<span data-ttu-id="4e5f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e5f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e5f6-111">name</span><span class="sxs-lookup"><span data-stu-id="4e5f6-111">name</span></span>|<span data-ttu-id="4e5f6-112">String</span><span class="sxs-lookup"><span data-stu-id="4e5f6-112">String</span></span>|<span data-ttu-id="4e5f6-113">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="4e5f6-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="4e5f6-114">value</span><span class="sxs-lookup"><span data-stu-id="4e5f6-114">value</span></span>|<span data-ttu-id="4e5f6-115">String</span><span class="sxs-lookup"><span data-stu-id="4e5f6-115">String</span></span>|<span data-ttu-id="4e5f6-116">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="4e5f6-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e5f6-117">关系</span><span class="sxs-lookup"><span data-stu-id="4e5f6-117">Relationships</span></span>
<span data-ttu-id="4e5f6-118">无</span><span class="sxs-lookup"><span data-stu-id="4e5f6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e5f6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e5f6-119">JSON Representation</span></span>
<span data-ttu-id="4e5f6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e5f6-120">Here is a JSON representation of the resource.</span></span>
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









