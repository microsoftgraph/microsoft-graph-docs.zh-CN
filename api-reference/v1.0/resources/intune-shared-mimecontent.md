---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
ms.openlocfilehash: 53776793fdd057ef057118decf2d72bb0b61a042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307061"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="503dd-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="503dd-103">mimeContent resource type</span></span>

> <span data-ttu-id="503dd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="503dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="503dd-105">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="503dd-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="503dd-106">属性</span><span class="sxs-lookup"><span data-stu-id="503dd-106">Properties</span></span>
|<span data-ttu-id="503dd-107">属性</span><span class="sxs-lookup"><span data-stu-id="503dd-107">Property</span></span>|<span data-ttu-id="503dd-108">类型</span><span class="sxs-lookup"><span data-stu-id="503dd-108">Type</span></span>|<span data-ttu-id="503dd-109">说明</span><span class="sxs-lookup"><span data-stu-id="503dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503dd-110">type</span><span class="sxs-lookup"><span data-stu-id="503dd-110">type</span></span>|<span data-ttu-id="503dd-111">String</span><span class="sxs-lookup"><span data-stu-id="503dd-111">String</span></span>|<span data-ttu-id="503dd-112">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="503dd-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="503dd-113">值</span><span class="sxs-lookup"><span data-stu-id="503dd-113">value</span></span>|<span data-ttu-id="503dd-114">Binary</span><span class="sxs-lookup"><span data-stu-id="503dd-114">Binary</span></span>|<span data-ttu-id="503dd-115">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="503dd-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="503dd-116">关系</span><span class="sxs-lookup"><span data-stu-id="503dd-116">Relationships</span></span>
<span data-ttu-id="503dd-117">无</span><span class="sxs-lookup"><span data-stu-id="503dd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="503dd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="503dd-118">JSON Representation</span></span>
<span data-ttu-id="503dd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="503dd-119">Here is a JSON representation of the resource.</span></span>
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



