---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a486753c95afce9dff6ceec5846ff618b9103b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971898"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="c8f72-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8f72-103">mimeContent resource type</span></span>

> <span data-ttu-id="c8f72-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c8f72-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8f72-105">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="c8f72-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="c8f72-106">属性</span><span class="sxs-lookup"><span data-stu-id="c8f72-106">Properties</span></span>
|<span data-ttu-id="c8f72-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8f72-107">Property</span></span>|<span data-ttu-id="c8f72-108">类型</span><span class="sxs-lookup"><span data-stu-id="c8f72-108">Type</span></span>|<span data-ttu-id="c8f72-109">说明</span><span class="sxs-lookup"><span data-stu-id="c8f72-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8f72-110">type</span><span class="sxs-lookup"><span data-stu-id="c8f72-110">type</span></span>|<span data-ttu-id="c8f72-111">String</span><span class="sxs-lookup"><span data-stu-id="c8f72-111">String</span></span>|<span data-ttu-id="c8f72-112">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="c8f72-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="c8f72-113">值</span><span class="sxs-lookup"><span data-stu-id="c8f72-113">value</span></span>|<span data-ttu-id="c8f72-114">Binary</span><span class="sxs-lookup"><span data-stu-id="c8f72-114">Binary</span></span>|<span data-ttu-id="c8f72-115">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="c8f72-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8f72-116">关系</span><span class="sxs-lookup"><span data-stu-id="c8f72-116">Relationships</span></span>
<span data-ttu-id="c8f72-117">无</span><span class="sxs-lookup"><span data-stu-id="c8f72-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8f72-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8f72-118">JSON Representation</span></span>
<span data-ttu-id="c8f72-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8f72-119">Here is a JSON representation of the resource.</span></span>
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



