---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f446983d5dfe101c89171baa776b32759726f279
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161654"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="23540-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="23540-103">mimeContent resource type</span></span>

> <span data-ttu-id="23540-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23540-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23540-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23540-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23540-106">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="23540-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="23540-107">属性</span><span class="sxs-lookup"><span data-stu-id="23540-107">Properties</span></span>
|<span data-ttu-id="23540-108">属性</span><span class="sxs-lookup"><span data-stu-id="23540-108">Property</span></span>|<span data-ttu-id="23540-109">类型</span><span class="sxs-lookup"><span data-stu-id="23540-109">Type</span></span>|<span data-ttu-id="23540-110">说明</span><span class="sxs-lookup"><span data-stu-id="23540-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23540-111">type</span><span class="sxs-lookup"><span data-stu-id="23540-111">type</span></span>|<span data-ttu-id="23540-112">String</span><span class="sxs-lookup"><span data-stu-id="23540-112">String</span></span>|<span data-ttu-id="23540-113">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="23540-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="23540-114">值</span><span class="sxs-lookup"><span data-stu-id="23540-114">value</span></span>|<span data-ttu-id="23540-115">Binary</span><span class="sxs-lookup"><span data-stu-id="23540-115">Binary</span></span>|<span data-ttu-id="23540-116">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="23540-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23540-117">关系</span><span class="sxs-lookup"><span data-stu-id="23540-117">Relationships</span></span>
<span data-ttu-id="23540-118">无</span><span class="sxs-lookup"><span data-stu-id="23540-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23540-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23540-119">JSON Representation</span></span>
<span data-ttu-id="23540-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23540-120">Here is a JSON representation of the resource.</span></span>
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




