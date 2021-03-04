---
author: swapnil1993
title: hyperlinkOrPictureColumn 资源类型
description: hyperlinkOrPictureColumn 资源指示列包含 URL 数据，这些数据可以是 achortag 或充当超链接的图像。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 937e3ba8b58213f6b4465c6bc618f4a3a95af5d5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446618"
---
# <a name="hyperlinkorpicturecolumn-resource-type"></a><span data-ttu-id="e623a-103">hyperlinkOrPictureColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="e623a-103">hyperlinkOrPictureColumn resource type</span></span>

<span data-ttu-id="e623a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e623a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="e623a-105">指示列包含 URL 数据，这些数据可以是 achortag 或充当超链接的图像。</span><span class="sxs-lookup"><span data-stu-id="e623a-105">Indicates that the column contains URL data which can be an achortag or an image that serves as a hyperlink.</span></span>


## <a name="properties"></a><span data-ttu-id="e623a-106">属性</span><span class="sxs-lookup"><span data-stu-id="e623a-106">Properties</span></span>

| <span data-ttu-id="e623a-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="e623a-107">Property name</span></span>      | <span data-ttu-id="e623a-108">类型</span><span class="sxs-lookup"><span data-stu-id="e623a-108">Type</span></span>               | <span data-ttu-id="e623a-109">说明</span><span class="sxs-lookup"><span data-stu-id="e623a-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="e623a-110">isPicture</span><span class="sxs-lookup"><span data-stu-id="e623a-110">isPicture</span></span>       | <span data-ttu-id="e623a-111">布尔</span><span class="sxs-lookup"><span data-stu-id="e623a-111">Boolean</span></span>             | <span data-ttu-id="e623a-112">指定用于 URL 列的显示格式是图像还是超链接。</span><span class="sxs-lookup"><span data-stu-id="e623a-112">Specifies whether the display format used for URL columns is an image or a hyperlink.</span></span> 


## <a name="json-representation"></a><span data-ttu-id="e623a-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e623a-113">JSON representation</span></span>

<span data-ttu-id="e623a-114">下面是 **hyperlinkOrPictureColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e623a-114">Here is a JSON representation of a **hyperlinkOrPictureColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" } -->

```json
{
  "isPicture": false
}
```