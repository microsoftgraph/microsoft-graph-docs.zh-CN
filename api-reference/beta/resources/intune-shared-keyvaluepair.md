---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d7b5551bf4ca3237c6a4fc08db51c8e08474c63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957898"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="51e51-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="51e51-103">keyValuePair resource type</span></span>

> <span data-ttu-id="51e51-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="51e51-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51e51-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="51e51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51e51-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="51e51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51e51-107">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="51e51-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="51e51-108">属性</span><span class="sxs-lookup"><span data-stu-id="51e51-108">Properties</span></span>
|<span data-ttu-id="51e51-109">属性</span><span class="sxs-lookup"><span data-stu-id="51e51-109">Property</span></span>|<span data-ttu-id="51e51-110">类型</span><span class="sxs-lookup"><span data-stu-id="51e51-110">Type</span></span>|<span data-ttu-id="51e51-111">说明</span><span class="sxs-lookup"><span data-stu-id="51e51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e51-112">name</span><span class="sxs-lookup"><span data-stu-id="51e51-112">name</span></span>|<span data-ttu-id="51e51-113">String</span><span class="sxs-lookup"><span data-stu-id="51e51-113">String</span></span>|<span data-ttu-id="51e51-114">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="51e51-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="51e51-115">值</span><span class="sxs-lookup"><span data-stu-id="51e51-115">value</span></span>|<span data-ttu-id="51e51-116">String</span><span class="sxs-lookup"><span data-stu-id="51e51-116">String</span></span>|<span data-ttu-id="51e51-117">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="51e51-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="51e51-118">关系</span><span class="sxs-lookup"><span data-stu-id="51e51-118">Relationships</span></span>
<span data-ttu-id="51e51-119">无</span><span class="sxs-lookup"><span data-stu-id="51e51-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51e51-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51e51-120">JSON Representation</span></span>
<span data-ttu-id="51e51-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51e51-121">Here is a JSON representation of the resource.</span></span>
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





