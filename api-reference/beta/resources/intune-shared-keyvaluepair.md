---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 056dbe1f8504a89e3551402de7aa7ff7bc0ce866
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858441"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="b6968-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6968-103">keyValuePair resource type</span></span>

> <span data-ttu-id="b6968-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6968-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6968-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6968-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6968-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b6968-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6968-107">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="b6968-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="b6968-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6968-108">Properties</span></span>
|<span data-ttu-id="b6968-109">属性</span><span class="sxs-lookup"><span data-stu-id="b6968-109">Property</span></span>|<span data-ttu-id="b6968-110">类型</span><span class="sxs-lookup"><span data-stu-id="b6968-110">Type</span></span>|<span data-ttu-id="b6968-111">说明</span><span class="sxs-lookup"><span data-stu-id="b6968-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6968-112">name</span><span class="sxs-lookup"><span data-stu-id="b6968-112">name</span></span>|<span data-ttu-id="b6968-113">String</span><span class="sxs-lookup"><span data-stu-id="b6968-113">String</span></span>|<span data-ttu-id="b6968-114">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="b6968-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="b6968-115">值</span><span class="sxs-lookup"><span data-stu-id="b6968-115">value</span></span>|<span data-ttu-id="b6968-116">String</span><span class="sxs-lookup"><span data-stu-id="b6968-116">String</span></span>|<span data-ttu-id="b6968-117">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="b6968-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6968-118">关系</span><span class="sxs-lookup"><span data-stu-id="b6968-118">Relationships</span></span>
<span data-ttu-id="b6968-119">无</span><span class="sxs-lookup"><span data-stu-id="b6968-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6968-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6968-120">JSON Representation</span></span>
<span data-ttu-id="b6968-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6968-121">Here is a JSON representation of the resource.</span></span>
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





