---
title: keyTypedValuePair 资源类型
description: 具有字符串键和类型化值的键-值对。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 392988272257bdaf7fc3e5b8bafd6d7ca652547d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955623"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="34182-103">keyTypedValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="34182-103">keyTypedValuePair resource type</span></span>

> <span data-ttu-id="34182-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34182-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34182-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34182-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34182-106">具有字符串键和类型化值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="34182-106">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="34182-107">属性</span><span class="sxs-lookup"><span data-stu-id="34182-107">Properties</span></span>
|<span data-ttu-id="34182-108">属性</span><span class="sxs-lookup"><span data-stu-id="34182-108">Property</span></span>|<span data-ttu-id="34182-109">类型</span><span class="sxs-lookup"><span data-stu-id="34182-109">Type</span></span>|<span data-ttu-id="34182-110">说明</span><span class="sxs-lookup"><span data-stu-id="34182-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34182-111">Key</span><span class="sxs-lookup"><span data-stu-id="34182-111">key</span></span>|<span data-ttu-id="34182-112">字符串</span><span class="sxs-lookup"><span data-stu-id="34182-112">String</span></span>|<span data-ttu-id="34182-113">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="34182-113">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34182-114">关系</span><span class="sxs-lookup"><span data-stu-id="34182-114">Relationships</span></span>
<span data-ttu-id="34182-115">无</span><span class="sxs-lookup"><span data-stu-id="34182-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34182-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34182-116">JSON Representation</span></span>
<span data-ttu-id="34182-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34182-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyTypedValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyTypedValuePair",
  "key": "String"
}
```



