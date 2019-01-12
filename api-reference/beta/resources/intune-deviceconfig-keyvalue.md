---
title: keyValue 资源类型
description: 键值定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5027388b455a41bc5895009a4ce79ca195ab8340
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957877"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="d6249-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6249-103">keyValue resource type</span></span>

> <span data-ttu-id="d6249-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6249-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6249-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6249-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6249-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d6249-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6249-107">键值定义。</span><span class="sxs-lookup"><span data-stu-id="d6249-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d6249-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6249-108">Properties</span></span>
|<span data-ttu-id="d6249-109">属性</span><span class="sxs-lookup"><span data-stu-id="d6249-109">Property</span></span>|<span data-ttu-id="d6249-110">类型</span><span class="sxs-lookup"><span data-stu-id="d6249-110">Type</span></span>|<span data-ttu-id="d6249-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6249-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6249-112">Key</span><span class="sxs-lookup"><span data-stu-id="d6249-112">key</span></span>|<span data-ttu-id="d6249-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d6249-113">String</span></span>|<span data-ttu-id="d6249-114">键。</span><span class="sxs-lookup"><span data-stu-id="d6249-114">Key.</span></span>|
|<span data-ttu-id="d6249-115">值</span><span class="sxs-lookup"><span data-stu-id="d6249-115">value</span></span>|<span data-ttu-id="d6249-116">String</span><span class="sxs-lookup"><span data-stu-id="d6249-116">String</span></span>|<span data-ttu-id="d6249-117">值。</span><span class="sxs-lookup"><span data-stu-id="d6249-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6249-118">关系</span><span class="sxs-lookup"><span data-stu-id="d6249-118">Relationships</span></span>
<span data-ttu-id="d6249-119">无</span><span class="sxs-lookup"><span data-stu-id="d6249-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6249-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6249-120">JSON Representation</span></span>
<span data-ttu-id="d6249-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6249-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





