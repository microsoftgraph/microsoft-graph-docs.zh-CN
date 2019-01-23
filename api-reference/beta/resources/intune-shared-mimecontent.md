---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62132b9e55b8130f82fc8414cbb6e90ba34bb70f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413456"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="50940-103">mimeContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="50940-103">mimeContent resource type</span></span>

> <span data-ttu-id="50940-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="50940-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50940-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="50940-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50940-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50940-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50940-107">包含通用 MIME 内容的属性。</span><span class="sxs-lookup"><span data-stu-id="50940-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="50940-108">属性</span><span class="sxs-lookup"><span data-stu-id="50940-108">Properties</span></span>
|<span data-ttu-id="50940-109">属性</span><span class="sxs-lookup"><span data-stu-id="50940-109">Property</span></span>|<span data-ttu-id="50940-110">类型</span><span class="sxs-lookup"><span data-stu-id="50940-110">Type</span></span>|<span data-ttu-id="50940-111">说明</span><span class="sxs-lookup"><span data-stu-id="50940-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50940-112">type</span><span class="sxs-lookup"><span data-stu-id="50940-112">type</span></span>|<span data-ttu-id="50940-113">String</span><span class="sxs-lookup"><span data-stu-id="50940-113">String</span></span>|<span data-ttu-id="50940-114">指示内容 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="50940-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="50940-115">值</span><span class="sxs-lookup"><span data-stu-id="50940-115">value</span></span>|<span data-ttu-id="50940-116">Binary</span><span class="sxs-lookup"><span data-stu-id="50940-116">Binary</span></span>|<span data-ttu-id="50940-117">包含实际内容的字节数组。</span><span class="sxs-lookup"><span data-stu-id="50940-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50940-118">关系</span><span class="sxs-lookup"><span data-stu-id="50940-118">Relationships</span></span>
<span data-ttu-id="50940-119">无</span><span class="sxs-lookup"><span data-stu-id="50940-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50940-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50940-120">JSON Representation</span></span>
<span data-ttu-id="50940-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50940-121">Here is a JSON representation of the resource.</span></span>
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




