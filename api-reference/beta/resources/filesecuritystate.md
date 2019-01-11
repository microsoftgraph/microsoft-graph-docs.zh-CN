---
title: fileSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 9d18021591b24d26577e41897111b90310746d18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869501"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="55cde-104">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="55cde-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="55cde-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55cde-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55cde-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55cde-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55cde-107">包含与通知相关的文件 （处理） 有关的信息。</span><span class="sxs-lookup"><span data-stu-id="55cde-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="55cde-108">属性</span><span class="sxs-lookup"><span data-stu-id="55cde-108">Properties</span></span>

| <span data-ttu-id="55cde-109">属性</span><span class="sxs-lookup"><span data-stu-id="55cde-109">Property</span></span>   | <span data-ttu-id="55cde-110">类型</span><span class="sxs-lookup"><span data-stu-id="55cde-110">Type</span></span>|<span data-ttu-id="55cde-111">Description</span><span class="sxs-lookup"><span data-stu-id="55cde-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55cde-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="55cde-112">fileHash</span></span>|[<span data-ttu-id="55cde-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="55cde-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="55cde-114">包含文件哈希 （加密和位置） 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="55cde-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="55cde-115">name</span><span class="sxs-lookup"><span data-stu-id="55cde-115">name</span></span>|<span data-ttu-id="55cde-116">字符串</span><span class="sxs-lookup"><span data-stu-id="55cde-116">String</span></span>|<span data-ttu-id="55cde-117">文件名 （不带路径）。</span><span class="sxs-lookup"><span data-stu-id="55cde-117">File name (without path).</span></span>|
|<span data-ttu-id="55cde-118">路径</span><span class="sxs-lookup"><span data-stu-id="55cde-118">path</span></span>|<span data-ttu-id="55cde-119">字符串</span><span class="sxs-lookup"><span data-stu-id="55cde-119">String</span></span>|<span data-ttu-id="55cde-120">文件/imageFile 完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="55cde-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="55cde-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="55cde-121">riskScore</span></span>|<span data-ttu-id="55cde-122">字符串</span><span class="sxs-lookup"><span data-stu-id="55cde-122">String</span></span>|<span data-ttu-id="55cde-123">提供程序生成/计算风险评分的警报的文件。</span><span class="sxs-lookup"><span data-stu-id="55cde-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="55cde-124">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="55cde-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55cde-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55cde-125">JSON representation</span></span>

<span data-ttu-id="55cde-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55cde-126">The following is a JSON representation of the resource.</span></span>

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
