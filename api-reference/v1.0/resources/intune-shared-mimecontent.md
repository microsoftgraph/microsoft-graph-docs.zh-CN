---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0b63289b3d7666eb27de7e6dc4e643dd9fa4772
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857041"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="463f9-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="463f9-103">mimeContent resource type</span></span>

> <span data-ttu-id="463f9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="463f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="463f9-105">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="463f9-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="463f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="463f9-106">Properties</span></span>
|<span data-ttu-id="463f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="463f9-107">Property</span></span>|<span data-ttu-id="463f9-108">类型</span><span class="sxs-lookup"><span data-stu-id="463f9-108">Type</span></span>|<span data-ttu-id="463f9-109">说明</span><span class="sxs-lookup"><span data-stu-id="463f9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="463f9-110">type</span><span class="sxs-lookup"><span data-stu-id="463f9-110">type</span></span>|<span data-ttu-id="463f9-111">String</span><span class="sxs-lookup"><span data-stu-id="463f9-111">String</span></span>|<span data-ttu-id="463f9-112">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="463f9-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="463f9-113">值</span><span class="sxs-lookup"><span data-stu-id="463f9-113">value</span></span>|<span data-ttu-id="463f9-114">Binary</span><span class="sxs-lookup"><span data-stu-id="463f9-114">Binary</span></span>|<span data-ttu-id="463f9-115">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="463f9-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="463f9-116">关系</span><span class="sxs-lookup"><span data-stu-id="463f9-116">Relationships</span></span>
<span data-ttu-id="463f9-117">无</span><span class="sxs-lookup"><span data-stu-id="463f9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="463f9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="463f9-118">JSON Representation</span></span>
<span data-ttu-id="463f9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="463f9-119">Here is a JSON representation of the resource.</span></span>
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



