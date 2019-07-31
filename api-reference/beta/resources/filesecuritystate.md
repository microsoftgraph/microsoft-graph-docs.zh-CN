---
title: fileSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f061ca71bcd16c16e0292673338e2cb8d915e845
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972010"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="22d87-104">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="22d87-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d87-105">包含有关与警报相关的文件 (不处理) 的信息。</span><span class="sxs-lookup"><span data-stu-id="22d87-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="22d87-106">属性</span><span class="sxs-lookup"><span data-stu-id="22d87-106">Properties</span></span>

| <span data-ttu-id="22d87-107">属性</span><span class="sxs-lookup"><span data-stu-id="22d87-107">Property</span></span>   | <span data-ttu-id="22d87-108">类型</span><span class="sxs-lookup"><span data-stu-id="22d87-108">Type</span></span>|<span data-ttu-id="22d87-109">说明</span><span class="sxs-lookup"><span data-stu-id="22d87-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d87-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="22d87-110">fileHash</span></span>|[<span data-ttu-id="22d87-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="22d87-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="22d87-112">包含文件哈希 (加密和位置敏感) 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="22d87-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="22d87-113">name</span><span class="sxs-lookup"><span data-stu-id="22d87-113">name</span></span>|<span data-ttu-id="22d87-114">String</span><span class="sxs-lookup"><span data-stu-id="22d87-114">String</span></span>|<span data-ttu-id="22d87-115">文件名 (不含路径)。</span><span class="sxs-lookup"><span data-stu-id="22d87-115">File name (without path).</span></span>|
|<span data-ttu-id="22d87-116">路径</span><span class="sxs-lookup"><span data-stu-id="22d87-116">path</span></span>|<span data-ttu-id="22d87-117">String</span><span class="sxs-lookup"><span data-stu-id="22d87-117">String</span></span>|<span data-ttu-id="22d87-118">文件/imageFile 的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="22d87-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="22d87-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="22d87-119">riskScore</span></span>|<span data-ttu-id="22d87-120">String</span><span class="sxs-lookup"><span data-stu-id="22d87-120">String</span></span>|<span data-ttu-id="22d87-121">通知文件的提供程序生成/计算风险分数。</span><span class="sxs-lookup"><span data-stu-id="22d87-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="22d87-122">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="22d87-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22d87-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22d87-123">JSON representation</span></span>

<span data-ttu-id="22d87-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22d87-124">The following is a JSON representation of the resource.</span></span>

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
