---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4360ce5a8873fde7d3286f55fc0c8993936a7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571875"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="585b7-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="585b7-103">mimeContent resource type</span></span>

> <span data-ttu-id="585b7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="585b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="585b7-105">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="585b7-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="585b7-106">属性</span><span class="sxs-lookup"><span data-stu-id="585b7-106">Properties</span></span>
|<span data-ttu-id="585b7-107">属性</span><span class="sxs-lookup"><span data-stu-id="585b7-107">Property</span></span>|<span data-ttu-id="585b7-108">类型</span><span class="sxs-lookup"><span data-stu-id="585b7-108">Type</span></span>|<span data-ttu-id="585b7-109">说明</span><span class="sxs-lookup"><span data-stu-id="585b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="585b7-110">type</span><span class="sxs-lookup"><span data-stu-id="585b7-110">type</span></span>|<span data-ttu-id="585b7-111">String</span><span class="sxs-lookup"><span data-stu-id="585b7-111">String</span></span>|<span data-ttu-id="585b7-112">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="585b7-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="585b7-113">value</span><span class="sxs-lookup"><span data-stu-id="585b7-113">value</span></span>|<span data-ttu-id="585b7-114">Binary</span><span class="sxs-lookup"><span data-stu-id="585b7-114">Binary</span></span>|<span data-ttu-id="585b7-115">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="585b7-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="585b7-116">关系</span><span class="sxs-lookup"><span data-stu-id="585b7-116">Relationships</span></span>
<span data-ttu-id="585b7-117">无</span><span class="sxs-lookup"><span data-stu-id="585b7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="585b7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="585b7-118">JSON Representation</span></span>
<span data-ttu-id="585b7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="585b7-119">Here is a JSON representation of the resource.</span></span>
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



