---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: tfitzmac
ms.openlocfilehash: 078d414330e7a6c333042b6f6eb83ec44e255d73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355071"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="80a59-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="80a59-103">keyValuePair resource type</span></span>

> <span data-ttu-id="80a59-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80a59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a59-105">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="80a59-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="80a59-106">属性</span><span class="sxs-lookup"><span data-stu-id="80a59-106">Properties</span></span>
|<span data-ttu-id="80a59-107">属性</span><span class="sxs-lookup"><span data-stu-id="80a59-107">Property</span></span>|<span data-ttu-id="80a59-108">类型</span><span class="sxs-lookup"><span data-stu-id="80a59-108">Type</span></span>|<span data-ttu-id="80a59-109">说明</span><span class="sxs-lookup"><span data-stu-id="80a59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a59-110">name</span><span class="sxs-lookup"><span data-stu-id="80a59-110">name</span></span>|<span data-ttu-id="80a59-111">String</span><span class="sxs-lookup"><span data-stu-id="80a59-111">String</span></span>|<span data-ttu-id="80a59-112">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="80a59-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="80a59-113">值</span><span class="sxs-lookup"><span data-stu-id="80a59-113">value</span></span>|<span data-ttu-id="80a59-114">String</span><span class="sxs-lookup"><span data-stu-id="80a59-114">String</span></span>|<span data-ttu-id="80a59-115">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="80a59-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="80a59-116">关系</span><span class="sxs-lookup"><span data-stu-id="80a59-116">Relationships</span></span>
<span data-ttu-id="80a59-117">无</span><span class="sxs-lookup"><span data-stu-id="80a59-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80a59-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80a59-118">JSON Representation</span></span>
<span data-ttu-id="80a59-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80a59-119">Here is a JSON representation of the resource.</span></span>
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



