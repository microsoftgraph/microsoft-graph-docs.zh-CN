---
title: numberRange 资源类型
description: 号码范围定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e47252b42fe7be886a1d6ce7c0d71b6c2dc1b21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460959"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="c3943-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3943-103">numberRange resource type</span></span>

<span data-ttu-id="c3943-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3943-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3943-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3943-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3943-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3943-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3943-107">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="c3943-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c3943-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3943-108">Properties</span></span>
|<span data-ttu-id="c3943-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3943-109">Property</span></span>|<span data-ttu-id="c3943-110">类型</span><span class="sxs-lookup"><span data-stu-id="c3943-110">Type</span></span>|<span data-ttu-id="c3943-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3943-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3943-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="c3943-112">lowerNumber</span></span>|<span data-ttu-id="c3943-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c3943-113">Int32</span></span>|<span data-ttu-id="c3943-114">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="c3943-114">Lower number.</span></span>|
|<span data-ttu-id="c3943-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="c3943-115">upperNumber</span></span>|<span data-ttu-id="c3943-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c3943-116">Int32</span></span>|<span data-ttu-id="c3943-117">上限数。</span><span class="sxs-lookup"><span data-stu-id="c3943-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3943-118">关系</span><span class="sxs-lookup"><span data-stu-id="c3943-118">Relationships</span></span>
<span data-ttu-id="c3943-119">无</span><span class="sxs-lookup"><span data-stu-id="c3943-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3943-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3943-120">JSON Representation</span></span>
<span data-ttu-id="c3943-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3943-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```



