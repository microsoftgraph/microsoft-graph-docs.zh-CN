---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef174774c345debe18b9a3d66075af6e439a4583
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367152"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="02091-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="02091-103">mimeContent resource type</span></span>

> <span data-ttu-id="02091-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02091-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02091-105">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="02091-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="02091-106">属性</span><span class="sxs-lookup"><span data-stu-id="02091-106">Properties</span></span>
|<span data-ttu-id="02091-107">属性</span><span class="sxs-lookup"><span data-stu-id="02091-107">Property</span></span>|<span data-ttu-id="02091-108">类型</span><span class="sxs-lookup"><span data-stu-id="02091-108">Type</span></span>|<span data-ttu-id="02091-109">说明</span><span class="sxs-lookup"><span data-stu-id="02091-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02091-110">type</span><span class="sxs-lookup"><span data-stu-id="02091-110">type</span></span>|<span data-ttu-id="02091-111">String</span><span class="sxs-lookup"><span data-stu-id="02091-111">String</span></span>|<span data-ttu-id="02091-112">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="02091-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="02091-113">value</span><span class="sxs-lookup"><span data-stu-id="02091-113">value</span></span>|<span data-ttu-id="02091-114">Binary</span><span class="sxs-lookup"><span data-stu-id="02091-114">Binary</span></span>|<span data-ttu-id="02091-115">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="02091-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02091-116">关系</span><span class="sxs-lookup"><span data-stu-id="02091-116">Relationships</span></span>
<span data-ttu-id="02091-117">无</span><span class="sxs-lookup"><span data-stu-id="02091-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02091-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02091-118">JSON Representation</span></span>
<span data-ttu-id="02091-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02091-119">Here is a JSON representation of the resource.</span></span>
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




