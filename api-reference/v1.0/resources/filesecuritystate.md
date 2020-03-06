---
title: fileSecurityState 资源类型
description: 包含有关与警报相关的文件（不处理）的信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc9d05e875104469a25ee742635ea8e86682d9e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531426"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="938ff-103">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="938ff-103">fileSecurityState resource type</span></span>

<span data-ttu-id="938ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="938ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="938ff-105">包含有关与警报相关的文件（不处理）的信息。</span><span class="sxs-lookup"><span data-stu-id="938ff-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="938ff-106">属性</span><span class="sxs-lookup"><span data-stu-id="938ff-106">Properties</span></span>

| <span data-ttu-id="938ff-107">属性</span><span class="sxs-lookup"><span data-stu-id="938ff-107">Property</span></span>   | <span data-ttu-id="938ff-108">类型</span><span class="sxs-lookup"><span data-stu-id="938ff-108">Type</span></span>|<span data-ttu-id="938ff-109">说明</span><span class="sxs-lookup"><span data-stu-id="938ff-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="938ff-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="938ff-110">fileHash</span></span>|[<span data-ttu-id="938ff-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="938ff-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="938ff-112">包含文件哈希（加密和位置敏感）的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="938ff-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="938ff-113">name</span><span class="sxs-lookup"><span data-stu-id="938ff-113">name</span></span>|<span data-ttu-id="938ff-114">字符串</span><span class="sxs-lookup"><span data-stu-id="938ff-114">String</span></span>|<span data-ttu-id="938ff-115">文件名（不含路径）。</span><span class="sxs-lookup"><span data-stu-id="938ff-115">File name (without path).</span></span>|
|<span data-ttu-id="938ff-116">路径</span><span class="sxs-lookup"><span data-stu-id="938ff-116">path</span></span>|<span data-ttu-id="938ff-117">String</span><span class="sxs-lookup"><span data-stu-id="938ff-117">String</span></span>|<span data-ttu-id="938ff-118">文件/imageFile 的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="938ff-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="938ff-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="938ff-119">riskScore</span></span>|<span data-ttu-id="938ff-120">字符串</span><span class="sxs-lookup"><span data-stu-id="938ff-120">String</span></span>|<span data-ttu-id="938ff-121">通知文件的提供程序生成/计算风险分数。</span><span class="sxs-lookup"><span data-stu-id="938ff-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="938ff-122">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="938ff-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="938ff-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="938ff-123">JSON representation</span></span>

<span data-ttu-id="938ff-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="938ff-124">The following is a JSON representation of the resource.</span></span>

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
