---
title: fileSecurityState 资源类型
description: 包含与通知相关的文件 （处理） 有关的信息。
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894094"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="50ffc-103">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="50ffc-103">fileSecurityState resource type</span></span>

<span data-ttu-id="50ffc-104">包含与通知相关的文件 （处理） 有关的信息。</span><span class="sxs-lookup"><span data-stu-id="50ffc-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="50ffc-105">属性</span><span class="sxs-lookup"><span data-stu-id="50ffc-105">Properties</span></span>

| <span data-ttu-id="50ffc-106">属性</span><span class="sxs-lookup"><span data-stu-id="50ffc-106">Property</span></span>   | <span data-ttu-id="50ffc-107">类型</span><span class="sxs-lookup"><span data-stu-id="50ffc-107">Type</span></span>|<span data-ttu-id="50ffc-108">Description</span><span class="sxs-lookup"><span data-stu-id="50ffc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50ffc-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="50ffc-109">fileHash</span></span>|[<span data-ttu-id="50ffc-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="50ffc-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="50ffc-111">包含文件哈希 （加密和位置） 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="50ffc-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="50ffc-112">name</span><span class="sxs-lookup"><span data-stu-id="50ffc-112">name</span></span>|<span data-ttu-id="50ffc-113">字符串</span><span class="sxs-lookup"><span data-stu-id="50ffc-113">String</span></span>|<span data-ttu-id="50ffc-114">文件名 （不带路径）。</span><span class="sxs-lookup"><span data-stu-id="50ffc-114">File name (without path).</span></span>|
|<span data-ttu-id="50ffc-115">路径</span><span class="sxs-lookup"><span data-stu-id="50ffc-115">path</span></span>|<span data-ttu-id="50ffc-116">字符串</span><span class="sxs-lookup"><span data-stu-id="50ffc-116">String</span></span>|<span data-ttu-id="50ffc-117">文件/imageFile 完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="50ffc-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="50ffc-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="50ffc-118">riskScore</span></span>|<span data-ttu-id="50ffc-119">字符串</span><span class="sxs-lookup"><span data-stu-id="50ffc-119">String</span></span>|<span data-ttu-id="50ffc-120">提供程序生成/计算风险评分的警报的文件。</span><span class="sxs-lookup"><span data-stu-id="50ffc-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="50ffc-121">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="50ffc-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50ffc-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50ffc-122">JSON representation</span></span>

<span data-ttu-id="50ffc-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50ffc-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
