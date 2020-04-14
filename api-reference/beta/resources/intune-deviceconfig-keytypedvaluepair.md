---
title: keyTypedValuePair 资源类型
description: 具有字符串键和类型化值的键-值对。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 651ba697eb6c6464bef8da327aadfe8fd0938081
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439904"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="b2495-103">keyTypedValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2495-103">keyTypedValuePair resource type</span></span>

<span data-ttu-id="b2495-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2495-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2495-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2495-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2495-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2495-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2495-107">具有字符串键和类型化值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="b2495-107">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="b2495-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2495-108">Properties</span></span>
|<span data-ttu-id="b2495-109">属性</span><span class="sxs-lookup"><span data-stu-id="b2495-109">Property</span></span>|<span data-ttu-id="b2495-110">类型</span><span class="sxs-lookup"><span data-stu-id="b2495-110">Type</span></span>|<span data-ttu-id="b2495-111">说明</span><span class="sxs-lookup"><span data-stu-id="b2495-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2495-112">Key</span><span class="sxs-lookup"><span data-stu-id="b2495-112">key</span></span>|<span data-ttu-id="b2495-113">String</span><span class="sxs-lookup"><span data-stu-id="b2495-113">String</span></span>|<span data-ttu-id="b2495-114">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="b2495-114">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2495-115">关系</span><span class="sxs-lookup"><span data-stu-id="b2495-115">Relationships</span></span>
<span data-ttu-id="b2495-116">无</span><span class="sxs-lookup"><span data-stu-id="b2495-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2495-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2495-117">JSON Representation</span></span>
<span data-ttu-id="b2495-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2495-118">Here is a JSON representation of the resource.</span></span>
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



