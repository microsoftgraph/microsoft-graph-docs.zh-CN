---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad580548e3f399a3c35d4f86e23eaab4dfa62979
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779991"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="147d7-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="147d7-103">mimeContent resource type</span></span>

> <span data-ttu-id="147d7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="147d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="147d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="147d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="147d7-106">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="147d7-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="147d7-107">属性</span><span class="sxs-lookup"><span data-stu-id="147d7-107">Properties</span></span>
|<span data-ttu-id="147d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="147d7-108">Property</span></span>|<span data-ttu-id="147d7-109">类型</span><span class="sxs-lookup"><span data-stu-id="147d7-109">Type</span></span>|<span data-ttu-id="147d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="147d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="147d7-111">类型</span><span class="sxs-lookup"><span data-stu-id="147d7-111">type</span></span>|<span data-ttu-id="147d7-112">String</span><span class="sxs-lookup"><span data-stu-id="147d7-112">String</span></span>|<span data-ttu-id="147d7-113">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="147d7-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="147d7-114">value</span><span class="sxs-lookup"><span data-stu-id="147d7-114">value</span></span>|<span data-ttu-id="147d7-115">Binary</span><span class="sxs-lookup"><span data-stu-id="147d7-115">Binary</span></span>|<span data-ttu-id="147d7-116">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="147d7-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="147d7-117">关系</span><span class="sxs-lookup"><span data-stu-id="147d7-117">Relationships</span></span>
<span data-ttu-id="147d7-118">无</span><span class="sxs-lookup"><span data-stu-id="147d7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="147d7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="147d7-119">JSON Representation</span></span>
<span data-ttu-id="147d7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="147d7-120">Here is a JSON representation of the resource.</span></span>
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





