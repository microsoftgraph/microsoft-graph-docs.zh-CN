---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
ms.openlocfilehash: 05088fa472c8f8a71adabbb0c807e7b2f0b80b09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333493"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="03b5d-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="03b5d-103">mimeContent resource type</span></span>

> <span data-ttu-id="03b5d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03b5d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03b5d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03b5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03b5d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="03b5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03b5d-107">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="03b5d-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="03b5d-108">属性</span><span class="sxs-lookup"><span data-stu-id="03b5d-108">Properties</span></span>
|<span data-ttu-id="03b5d-109">属性</span><span class="sxs-lookup"><span data-stu-id="03b5d-109">Property</span></span>|<span data-ttu-id="03b5d-110">类型</span><span class="sxs-lookup"><span data-stu-id="03b5d-110">Type</span></span>|<span data-ttu-id="03b5d-111">说明</span><span class="sxs-lookup"><span data-stu-id="03b5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03b5d-112">type</span><span class="sxs-lookup"><span data-stu-id="03b5d-112">type</span></span>|<span data-ttu-id="03b5d-113">String</span><span class="sxs-lookup"><span data-stu-id="03b5d-113">String</span></span>|<span data-ttu-id="03b5d-114">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="03b5d-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="03b5d-115">值</span><span class="sxs-lookup"><span data-stu-id="03b5d-115">value</span></span>|<span data-ttu-id="03b5d-116">Binary</span><span class="sxs-lookup"><span data-stu-id="03b5d-116">Binary</span></span>|<span data-ttu-id="03b5d-117">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="03b5d-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03b5d-118">关系</span><span class="sxs-lookup"><span data-stu-id="03b5d-118">Relationships</span></span>
<span data-ttu-id="03b5d-119">无</span><span class="sxs-lookup"><span data-stu-id="03b5d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03b5d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03b5d-120">JSON Representation</span></span>
<span data-ttu-id="03b5d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03b5d-121">Here is a JSON representation of the resource.</span></span>
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





