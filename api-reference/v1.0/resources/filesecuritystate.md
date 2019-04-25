---
title: fileSecurityState 资源类型
description: 包含有关与警报相关的文件 (不处理) 的信息。
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564790"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="62cf0-103">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="62cf0-103">fileSecurityState resource type</span></span>

<span data-ttu-id="62cf0-104">包含有关与警报相关的文件 (不处理) 的信息。</span><span class="sxs-lookup"><span data-stu-id="62cf0-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="62cf0-105">属性</span><span class="sxs-lookup"><span data-stu-id="62cf0-105">Properties</span></span>

| <span data-ttu-id="62cf0-106">属性</span><span class="sxs-lookup"><span data-stu-id="62cf0-106">Property</span></span>   | <span data-ttu-id="62cf0-107">类型</span><span class="sxs-lookup"><span data-stu-id="62cf0-107">Type</span></span>|<span data-ttu-id="62cf0-108">说明</span><span class="sxs-lookup"><span data-stu-id="62cf0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62cf0-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="62cf0-109">fileHash</span></span>|[<span data-ttu-id="62cf0-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="62cf0-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="62cf0-111">包含文件哈希 (加密和位置敏感) 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="62cf0-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="62cf0-112">name</span><span class="sxs-lookup"><span data-stu-id="62cf0-112">name</span></span>|<span data-ttu-id="62cf0-113">String</span><span class="sxs-lookup"><span data-stu-id="62cf0-113">String</span></span>|<span data-ttu-id="62cf0-114">文件名 (不含路径)。</span><span class="sxs-lookup"><span data-stu-id="62cf0-114">File name (without path).</span></span>|
|<span data-ttu-id="62cf0-115">路径</span><span class="sxs-lookup"><span data-stu-id="62cf0-115">path</span></span>|<span data-ttu-id="62cf0-116">String</span><span class="sxs-lookup"><span data-stu-id="62cf0-116">String</span></span>|<span data-ttu-id="62cf0-117">文件/imageFile 的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="62cf0-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="62cf0-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="62cf0-118">riskScore</span></span>|<span data-ttu-id="62cf0-119">String</span><span class="sxs-lookup"><span data-stu-id="62cf0-119">String</span></span>|<span data-ttu-id="62cf0-120">通知文件的提供程序生成/计算风险分数。</span><span class="sxs-lookup"><span data-stu-id="62cf0-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="62cf0-121">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="62cf0-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62cf0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62cf0-122">JSON representation</span></span>

<span data-ttu-id="62cf0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62cf0-123">The following is a JSON representation of the resource.</span></span>

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
