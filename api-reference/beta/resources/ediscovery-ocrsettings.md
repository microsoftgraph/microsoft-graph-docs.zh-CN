---
title: ocrSettings 资源类型
description: 电子数据展示案例的 OCR 设置
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 648e0ad63f558f211591d1c8aa976c2689dd271d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080746"
---
# <a name="ocrsettings-resource-type"></a><span data-ttu-id="78156-103">ocrSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="78156-103">ocrSettings resource type</span></span>

<span data-ttu-id="78156-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="78156-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78156-105">OCR (光学字符识别) 电子数据展示案例的设置。</span><span class="sxs-lookup"><span data-stu-id="78156-105">The OCR (Optical Character Recognition) settings for the eDiscovery case.</span></span>

## <a name="properties"></a><span data-ttu-id="78156-106">属性</span><span class="sxs-lookup"><span data-stu-id="78156-106">Properties</span></span>

|<span data-ttu-id="78156-107">属性</span><span class="sxs-lookup"><span data-stu-id="78156-107">Property</span></span>|<span data-ttu-id="78156-108">类型</span><span class="sxs-lookup"><span data-stu-id="78156-108">Type</span></span>|<span data-ttu-id="78156-109">说明</span><span class="sxs-lookup"><span data-stu-id="78156-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78156-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="78156-110">isEnabled</span></span>|<span data-ttu-id="78156-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="78156-111">Boolean</span></span>|<span data-ttu-id="78156-112">指示是否对案例启用 OCR。</span><span class="sxs-lookup"><span data-stu-id="78156-112">Indicates whether or not OCR is enabled for the case.</span></span>|
|<span data-ttu-id="78156-113">maxImageSize</span><span class="sxs-lookup"><span data-stu-id="78156-113">maxImageSize</span></span>|<span data-ttu-id="78156-114">Int32</span><span class="sxs-lookup"><span data-stu-id="78156-114">Int32</span></span>|<span data-ttu-id="78156-115">将处理的最大图像大小（以 KB 为单位) 。</span><span class="sxs-lookup"><span data-stu-id="78156-115">Maximum image size that will be processed in KB).</span></span>|
|<span data-ttu-id="78156-116">timeout</span><span class="sxs-lookup"><span data-stu-id="78156-116">timeout</span></span>|<span data-ttu-id="78156-117">期限</span><span class="sxs-lookup"><span data-stu-id="78156-117">Duration</span></span>|<span data-ttu-id="78156-118">OCR 引擎的超时持续时间。</span><span class="sxs-lookup"><span data-stu-id="78156-118">The timeout duration for the OCR engine.</span></span> <span data-ttu-id="78156-119">较长的超时可能会增加 OCR 的成功，但会增加总处理时间。</span><span class="sxs-lookup"><span data-stu-id="78156-119">A longer timeout may increase success of OCR, but may add to the total processing time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78156-120">关系</span><span class="sxs-lookup"><span data-stu-id="78156-120">Relationships</span></span>

<span data-ttu-id="78156-121">无。</span><span class="sxs-lookup"><span data-stu-id="78156-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78156-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78156-122">JSON representation</span></span>

<span data-ttu-id="78156-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78156-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```
