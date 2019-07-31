---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f548cf98adba98518fcbc0f3c4b06b583ff5e234
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967355"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="08f71-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="08f71-103">mimeContent resource type</span></span>

> <span data-ttu-id="08f71-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08f71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08f71-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08f71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08f71-106">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="08f71-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="08f71-107">属性</span><span class="sxs-lookup"><span data-stu-id="08f71-107">Properties</span></span>
|<span data-ttu-id="08f71-108">属性</span><span class="sxs-lookup"><span data-stu-id="08f71-108">Property</span></span>|<span data-ttu-id="08f71-109">类型</span><span class="sxs-lookup"><span data-stu-id="08f71-109">Type</span></span>|<span data-ttu-id="08f71-110">说明</span><span class="sxs-lookup"><span data-stu-id="08f71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f71-111">type</span><span class="sxs-lookup"><span data-stu-id="08f71-111">type</span></span>|<span data-ttu-id="08f71-112">String</span><span class="sxs-lookup"><span data-stu-id="08f71-112">String</span></span>|<span data-ttu-id="08f71-113">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="08f71-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="08f71-114">value</span><span class="sxs-lookup"><span data-stu-id="08f71-114">value</span></span>|<span data-ttu-id="08f71-115">Binary</span><span class="sxs-lookup"><span data-stu-id="08f71-115">Binary</span></span>|<span data-ttu-id="08f71-116">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="08f71-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08f71-117">关系</span><span class="sxs-lookup"><span data-stu-id="08f71-117">Relationships</span></span>
<span data-ttu-id="08f71-118">无</span><span class="sxs-lookup"><span data-stu-id="08f71-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08f71-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08f71-119">JSON Representation</span></span>
<span data-ttu-id="08f71-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08f71-120">Here is a JSON representation of the resource.</span></span>
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





