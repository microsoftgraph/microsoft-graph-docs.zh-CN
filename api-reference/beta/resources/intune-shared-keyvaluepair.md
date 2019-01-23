---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f31e83c5e53ea4c2873fd2b425cc0e0c02678ea7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415780"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="e1f36-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1f36-103">keyValuePair resource type</span></span>

> <span data-ttu-id="e1f36-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e1f36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1f36-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1f36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1f36-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1f36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1f36-107">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="e1f36-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="e1f36-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1f36-108">Properties</span></span>
|<span data-ttu-id="e1f36-109">属性</span><span class="sxs-lookup"><span data-stu-id="e1f36-109">Property</span></span>|<span data-ttu-id="e1f36-110">类型</span><span class="sxs-lookup"><span data-stu-id="e1f36-110">Type</span></span>|<span data-ttu-id="e1f36-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1f36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1f36-112">name</span><span class="sxs-lookup"><span data-stu-id="e1f36-112">name</span></span>|<span data-ttu-id="e1f36-113">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-113">String</span></span>|<span data-ttu-id="e1f36-114">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="e1f36-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="e1f36-115">值</span><span class="sxs-lookup"><span data-stu-id="e1f36-115">value</span></span>|<span data-ttu-id="e1f36-116">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-116">String</span></span>|<span data-ttu-id="e1f36-117">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="e1f36-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1f36-118">关系</span><span class="sxs-lookup"><span data-stu-id="e1f36-118">Relationships</span></span>
<span data-ttu-id="e1f36-119">无</span><span class="sxs-lookup"><span data-stu-id="e1f36-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1f36-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1f36-120">JSON Representation</span></span>
<span data-ttu-id="e1f36-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1f36-121">Here is a JSON representation of the resource.</span></span>
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




