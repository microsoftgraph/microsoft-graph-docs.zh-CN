---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44f1765fb4f03a287665fe4ed1faef7012a43459
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805892"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="2fc41-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fc41-103">keyValuePair resource type</span></span>

> <span data-ttu-id="2fc41-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2fc41-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fc41-105">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="2fc41-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="2fc41-106">属性</span><span class="sxs-lookup"><span data-stu-id="2fc41-106">Properties</span></span>
|<span data-ttu-id="2fc41-107">属性</span><span class="sxs-lookup"><span data-stu-id="2fc41-107">Property</span></span>|<span data-ttu-id="2fc41-108">类型</span><span class="sxs-lookup"><span data-stu-id="2fc41-108">Type</span></span>|<span data-ttu-id="2fc41-109">说明</span><span class="sxs-lookup"><span data-stu-id="2fc41-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc41-110">name</span><span class="sxs-lookup"><span data-stu-id="2fc41-110">name</span></span>|<span data-ttu-id="2fc41-111">String</span><span class="sxs-lookup"><span data-stu-id="2fc41-111">String</span></span>|<span data-ttu-id="2fc41-112">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="2fc41-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="2fc41-113">值</span><span class="sxs-lookup"><span data-stu-id="2fc41-113">value</span></span>|<span data-ttu-id="2fc41-114">String</span><span class="sxs-lookup"><span data-stu-id="2fc41-114">String</span></span>|<span data-ttu-id="2fc41-115">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="2fc41-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fc41-116">关系</span><span class="sxs-lookup"><span data-stu-id="2fc41-116">Relationships</span></span>
<span data-ttu-id="2fc41-117">无</span><span class="sxs-lookup"><span data-stu-id="2fc41-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fc41-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fc41-118">JSON Representation</span></span>
<span data-ttu-id="2fc41-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fc41-119">Here is a JSON representation of the resource.</span></span>
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



