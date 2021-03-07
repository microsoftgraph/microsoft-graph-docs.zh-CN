---
author: nilakhan
description: 表示打印文档上载的信息
title: printDocumentUploadProperties 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: e877901b842670e09cb283b40613a1185aabaafe
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517193"
---
# <a name="printdocumentuploadproperties-resource-type"></a><span data-ttu-id="697c6-103">printDocumentUploadProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="697c6-103">printDocumentUploadProperties resource type</span></span>

<span data-ttu-id="697c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="697c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="697c6-105">描述正在上载的文档</span><span class="sxs-lookup"><span data-stu-id="697c6-105">Describes the document that is being uploaded</span></span>

## <a name="properties"></a><span data-ttu-id="697c6-106">属性</span><span class="sxs-lookup"><span data-stu-id="697c6-106">Properties</span></span>
|<span data-ttu-id="697c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="697c6-107">Property</span></span>|<span data-ttu-id="697c6-108">类型</span><span class="sxs-lookup"><span data-stu-id="697c6-108">Type</span></span>|<span data-ttu-id="697c6-109">说明</span><span class="sxs-lookup"><span data-stu-id="697c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="697c6-110">contentType</span><span class="sxs-lookup"><span data-stu-id="697c6-110">contentType</span></span>|<span data-ttu-id="697c6-111">String</span><span class="sxs-lookup"><span data-stu-id="697c6-111">String</span></span>|<span data-ttu-id="697c6-112">文档的内容 (MIME) 类型。</span><span class="sxs-lookup"><span data-stu-id="697c6-112">The document's content (MIME) type.</span></span>|
|<span data-ttu-id="697c6-113">documentName</span><span class="sxs-lookup"><span data-stu-id="697c6-113">documentName</span></span>|<span data-ttu-id="697c6-114">String</span><span class="sxs-lookup"><span data-stu-id="697c6-114">String</span></span>|<span data-ttu-id="697c6-115">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="697c6-115">The document's name.</span></span>|
|<span data-ttu-id="697c6-116">size</span><span class="sxs-lookup"><span data-stu-id="697c6-116">size</span></span>|<span data-ttu-id="697c6-117">Int64</span><span class="sxs-lookup"><span data-stu-id="697c6-117">Int64</span></span>|<span data-ttu-id="697c6-118">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="697c6-118">The document's size in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="697c6-119">关系</span><span class="sxs-lookup"><span data-stu-id="697c6-119">Relationships</span></span>
<span data-ttu-id="697c6-120">无。</span><span class="sxs-lookup"><span data-stu-id="697c6-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="697c6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="697c6-121">JSON representation</span></span>
<span data-ttu-id="697c6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="697c6-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printDocumentUploadProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocumentUploadProperties",
  "contentType": "String",
  "documentName": "String",
  "size": "Integer"
}
```

