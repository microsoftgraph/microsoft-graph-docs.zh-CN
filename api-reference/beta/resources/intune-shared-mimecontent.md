---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 826606d41feb0f0a156a1b8240bde7f4ac926a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838225"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="859c1-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="859c1-103">mimeContent resource type</span></span>

> <span data-ttu-id="859c1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="859c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="859c1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="859c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="859c1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="859c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="859c1-107">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="859c1-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="859c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="859c1-108">Properties</span></span>
|<span data-ttu-id="859c1-109">属性</span><span class="sxs-lookup"><span data-stu-id="859c1-109">Property</span></span>|<span data-ttu-id="859c1-110">类型</span><span class="sxs-lookup"><span data-stu-id="859c1-110">Type</span></span>|<span data-ttu-id="859c1-111">说明</span><span class="sxs-lookup"><span data-stu-id="859c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="859c1-112">type</span><span class="sxs-lookup"><span data-stu-id="859c1-112">type</span></span>|<span data-ttu-id="859c1-113">String</span><span class="sxs-lookup"><span data-stu-id="859c1-113">String</span></span>|<span data-ttu-id="859c1-114">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="859c1-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="859c1-115">值</span><span class="sxs-lookup"><span data-stu-id="859c1-115">value</span></span>|<span data-ttu-id="859c1-116">Binary</span><span class="sxs-lookup"><span data-stu-id="859c1-116">Binary</span></span>|<span data-ttu-id="859c1-117">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="859c1-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="859c1-118">关系</span><span class="sxs-lookup"><span data-stu-id="859c1-118">Relationships</span></span>
<span data-ttu-id="859c1-119">无</span><span class="sxs-lookup"><span data-stu-id="859c1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="859c1-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="859c1-120">JSON Representation</span></span>
<span data-ttu-id="859c1-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="859c1-121">Here is a JSON representation of the resource.</span></span>
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





