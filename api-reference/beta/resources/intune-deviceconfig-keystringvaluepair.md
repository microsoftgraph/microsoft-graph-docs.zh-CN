---
title: keyStringValuePair 资源类型
description: 带有字符串键和字符串值的键-值对。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ad2380d84a329d2bfaf9359128944e90a90c393
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529784"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="2c0dd-103">keyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c0dd-103">keyStringValuePair resource type</span></span>

<span data-ttu-id="2c0dd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2c0dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c0dd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c0dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c0dd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c0dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0dd-107">带有字符串键和字符串值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="2c0dd-107">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="2c0dd-108">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2c0dd-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c0dd-109">属性</span><span class="sxs-lookup"><span data-stu-id="2c0dd-109">Properties</span></span>
|<span data-ttu-id="2c0dd-110">属性</span><span class="sxs-lookup"><span data-stu-id="2c0dd-110">Property</span></span>|<span data-ttu-id="2c0dd-111">类型</span><span class="sxs-lookup"><span data-stu-id="2c0dd-111">Type</span></span>|<span data-ttu-id="2c0dd-112">说明</span><span class="sxs-lookup"><span data-stu-id="2c0dd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0dd-113">Key</span><span class="sxs-lookup"><span data-stu-id="2c0dd-113">key</span></span>|<span data-ttu-id="2c0dd-114">String</span><span class="sxs-lookup"><span data-stu-id="2c0dd-114">String</span></span>|<span data-ttu-id="2c0dd-115">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="2c0dd-115">The string key of the key-value pair.</span></span> <span data-ttu-id="2c0dd-116">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2c0dd-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="2c0dd-117">value</span><span class="sxs-lookup"><span data-stu-id="2c0dd-117">value</span></span>|<span data-ttu-id="2c0dd-118">String</span><span class="sxs-lookup"><span data-stu-id="2c0dd-118">String</span></span>|<span data-ttu-id="2c0dd-119">键/值对的字符串值。</span><span class="sxs-lookup"><span data-stu-id="2c0dd-119">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c0dd-120">关系</span><span class="sxs-lookup"><span data-stu-id="2c0dd-120">Relationships</span></span>
<span data-ttu-id="2c0dd-121">无</span><span class="sxs-lookup"><span data-stu-id="2c0dd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c0dd-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c0dd-122">JSON Representation</span></span>
<span data-ttu-id="2c0dd-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c0dd-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



