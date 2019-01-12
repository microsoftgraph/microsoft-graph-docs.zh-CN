---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926440"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="c6068-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6068-103">keyValuePair resource type</span></span>

> <span data-ttu-id="c6068-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6068-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6068-105">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="c6068-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="c6068-106">属性</span><span class="sxs-lookup"><span data-stu-id="c6068-106">Properties</span></span>
|<span data-ttu-id="c6068-107">属性</span><span class="sxs-lookup"><span data-stu-id="c6068-107">Property</span></span>|<span data-ttu-id="c6068-108">类型</span><span class="sxs-lookup"><span data-stu-id="c6068-108">Type</span></span>|<span data-ttu-id="c6068-109">说明</span><span class="sxs-lookup"><span data-stu-id="c6068-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6068-110">name</span><span class="sxs-lookup"><span data-stu-id="c6068-110">name</span></span>|<span data-ttu-id="c6068-111">String</span><span class="sxs-lookup"><span data-stu-id="c6068-111">String</span></span>|<span data-ttu-id="c6068-112">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="c6068-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="c6068-113">值</span><span class="sxs-lookup"><span data-stu-id="c6068-113">value</span></span>|<span data-ttu-id="c6068-114">String</span><span class="sxs-lookup"><span data-stu-id="c6068-114">String</span></span>|<span data-ttu-id="c6068-115">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="c6068-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6068-116">关系</span><span class="sxs-lookup"><span data-stu-id="c6068-116">Relationships</span></span>
<span data-ttu-id="c6068-117">无</span><span class="sxs-lookup"><span data-stu-id="c6068-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6068-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6068-118">JSON Representation</span></span>
<span data-ttu-id="c6068-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6068-119">Here is a JSON representation of the resource.</span></span>
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



