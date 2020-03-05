---
title: fileSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3827562407b0c253c1d5a16ff26071e8500010bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498166"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="09315-104">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="09315-104">fileSecurityState resource type</span></span>

<span data-ttu-id="09315-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09315-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09315-106">包含有关与警报相关的文件（不处理）的信息。</span><span class="sxs-lookup"><span data-stu-id="09315-106">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="09315-107">属性</span><span class="sxs-lookup"><span data-stu-id="09315-107">Properties</span></span>

| <span data-ttu-id="09315-108">属性</span><span class="sxs-lookup"><span data-stu-id="09315-108">Property</span></span>   | <span data-ttu-id="09315-109">类型</span><span class="sxs-lookup"><span data-stu-id="09315-109">Type</span></span>|<span data-ttu-id="09315-110">说明</span><span class="sxs-lookup"><span data-stu-id="09315-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09315-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="09315-111">fileHash</span></span>|[<span data-ttu-id="09315-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="09315-112">fileHash</span></span>](filehash.md)|<span data-ttu-id="09315-113">包含文件哈希（加密和位置敏感）的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="09315-113">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="09315-114">name</span><span class="sxs-lookup"><span data-stu-id="09315-114">name</span></span>|<span data-ttu-id="09315-115">String</span><span class="sxs-lookup"><span data-stu-id="09315-115">String</span></span>|<span data-ttu-id="09315-116">文件名（不含路径）。</span><span class="sxs-lookup"><span data-stu-id="09315-116">File name (without path).</span></span>|
|<span data-ttu-id="09315-117">路径</span><span class="sxs-lookup"><span data-stu-id="09315-117">path</span></span>|<span data-ttu-id="09315-118">String</span><span class="sxs-lookup"><span data-stu-id="09315-118">String</span></span>|<span data-ttu-id="09315-119">文件/imageFile 的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="09315-119">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="09315-120">riskScore</span><span class="sxs-lookup"><span data-stu-id="09315-120">riskScore</span></span>|<span data-ttu-id="09315-121">String</span><span class="sxs-lookup"><span data-stu-id="09315-121">String</span></span>|<span data-ttu-id="09315-122">通知文件的提供程序生成/计算风险分数。</span><span class="sxs-lookup"><span data-stu-id="09315-122">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="09315-123">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="09315-123">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09315-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09315-124">JSON representation</span></span>

<span data-ttu-id="09315-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09315-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
