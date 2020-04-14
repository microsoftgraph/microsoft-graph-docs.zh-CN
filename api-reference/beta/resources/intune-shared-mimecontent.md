---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86537f6d93f2ff50c212105fce3f4fb91f137184
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466164"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="95540-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="95540-103">mimeContent resource type</span></span>

<span data-ttu-id="95540-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95540-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95540-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95540-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95540-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95540-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95540-107">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="95540-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="95540-108">属性</span><span class="sxs-lookup"><span data-stu-id="95540-108">Properties</span></span>
|<span data-ttu-id="95540-109">属性</span><span class="sxs-lookup"><span data-stu-id="95540-109">Property</span></span>|<span data-ttu-id="95540-110">类型</span><span class="sxs-lookup"><span data-stu-id="95540-110">Type</span></span>|<span data-ttu-id="95540-111">说明</span><span class="sxs-lookup"><span data-stu-id="95540-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95540-112">type</span><span class="sxs-lookup"><span data-stu-id="95540-112">type</span></span>|<span data-ttu-id="95540-113">String</span><span class="sxs-lookup"><span data-stu-id="95540-113">String</span></span>|<span data-ttu-id="95540-114">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="95540-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="95540-115">value</span><span class="sxs-lookup"><span data-stu-id="95540-115">value</span></span>|<span data-ttu-id="95540-116">Binary</span><span class="sxs-lookup"><span data-stu-id="95540-116">Binary</span></span>|<span data-ttu-id="95540-117">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="95540-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95540-118">关系</span><span class="sxs-lookup"><span data-stu-id="95540-118">Relationships</span></span>
<span data-ttu-id="95540-119">无</span><span class="sxs-lookup"><span data-stu-id="95540-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95540-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95540-120">JSON Representation</span></span>
<span data-ttu-id="95540-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95540-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



