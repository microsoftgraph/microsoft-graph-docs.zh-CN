---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e17fd6abb6470fe46c836f7ed4b9f38362abb74d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751550"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="a87c5-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a87c5-103">mimeContent resource type</span></span>

<span data-ttu-id="a87c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a87c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a87c5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a87c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a87c5-106">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="a87c5-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="a87c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="a87c5-107">Properties</span></span>
|<span data-ttu-id="a87c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="a87c5-108">Property</span></span>|<span data-ttu-id="a87c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="a87c5-109">Type</span></span>|<span data-ttu-id="a87c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="a87c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a87c5-111">type</span><span class="sxs-lookup"><span data-stu-id="a87c5-111">type</span></span>|<span data-ttu-id="a87c5-112">String</span><span class="sxs-lookup"><span data-stu-id="a87c5-112">String</span></span>|<span data-ttu-id="a87c5-113">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="a87c5-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="a87c5-114">value</span><span class="sxs-lookup"><span data-stu-id="a87c5-114">value</span></span>|<span data-ttu-id="a87c5-115">Binary</span><span class="sxs-lookup"><span data-stu-id="a87c5-115">Binary</span></span>|<span data-ttu-id="a87c5-116">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="a87c5-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a87c5-117">关系</span><span class="sxs-lookup"><span data-stu-id="a87c5-117">Relationships</span></span>
<span data-ttu-id="a87c5-118">无</span><span class="sxs-lookup"><span data-stu-id="a87c5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a87c5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a87c5-119">JSON Representation</span></span>
<span data-ttu-id="a87c5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a87c5-120">Here is a JSON representation of the resource.</span></span>
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




