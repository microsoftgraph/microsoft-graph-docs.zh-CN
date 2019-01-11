---
title: keyValue 资源类型
description: 键值定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aae0fea85c5dd4f647a72c0fe66890bd8b82520b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885013"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="be46d-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="be46d-103">keyValue resource type</span></span>

> <span data-ttu-id="be46d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="be46d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be46d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be46d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be46d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="be46d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be46d-107">键值定义。</span><span class="sxs-lookup"><span data-stu-id="be46d-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="be46d-108">属性</span><span class="sxs-lookup"><span data-stu-id="be46d-108">Properties</span></span>
|<span data-ttu-id="be46d-109">属性</span><span class="sxs-lookup"><span data-stu-id="be46d-109">Property</span></span>|<span data-ttu-id="be46d-110">类型</span><span class="sxs-lookup"><span data-stu-id="be46d-110">Type</span></span>|<span data-ttu-id="be46d-111">说明</span><span class="sxs-lookup"><span data-stu-id="be46d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be46d-112">Key</span><span class="sxs-lookup"><span data-stu-id="be46d-112">key</span></span>|<span data-ttu-id="be46d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="be46d-113">String</span></span>|<span data-ttu-id="be46d-114">键。</span><span class="sxs-lookup"><span data-stu-id="be46d-114">Key.</span></span>|
|<span data-ttu-id="be46d-115">值</span><span class="sxs-lookup"><span data-stu-id="be46d-115">value</span></span>|<span data-ttu-id="be46d-116">String</span><span class="sxs-lookup"><span data-stu-id="be46d-116">String</span></span>|<span data-ttu-id="be46d-117">值。</span><span class="sxs-lookup"><span data-stu-id="be46d-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be46d-118">关系</span><span class="sxs-lookup"><span data-stu-id="be46d-118">Relationships</span></span>
<span data-ttu-id="be46d-119">无</span><span class="sxs-lookup"><span data-stu-id="be46d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be46d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be46d-120">JSON Representation</span></span>
<span data-ttu-id="be46d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be46d-121">Here is a JSON representation of the resource.</span></span>
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





