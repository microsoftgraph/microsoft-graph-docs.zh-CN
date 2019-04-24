---
title: fileSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506406"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="6b7d6-104">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b7d6-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b7d6-105">包含有关与警报相关的文件 (不处理) 的信息。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="6b7d6-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b7d6-106">Properties</span></span>

| <span data-ttu-id="6b7d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b7d6-107">Property</span></span>   | <span data-ttu-id="6b7d6-108">类型</span><span class="sxs-lookup"><span data-stu-id="6b7d6-108">Type</span></span>|<span data-ttu-id="6b7d6-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b7d6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b7d6-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="6b7d6-110">fileHash</span></span>|[<span data-ttu-id="6b7d6-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="6b7d6-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="6b7d6-112">包含文件哈希 (加密和位置敏感) 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="6b7d6-113">name</span><span class="sxs-lookup"><span data-stu-id="6b7d6-113">name</span></span>|<span data-ttu-id="6b7d6-114">String</span><span class="sxs-lookup"><span data-stu-id="6b7d6-114">String</span></span>|<span data-ttu-id="6b7d6-115">文件名 (不含路径)。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-115">File name (without path).</span></span>|
|<span data-ttu-id="6b7d6-116">路径</span><span class="sxs-lookup"><span data-stu-id="6b7d6-116">path</span></span>|<span data-ttu-id="6b7d6-117">String</span><span class="sxs-lookup"><span data-stu-id="6b7d6-117">String</span></span>|<span data-ttu-id="6b7d6-118">文件/imageFile 的完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="6b7d6-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="6b7d6-119">riskScore</span></span>|<span data-ttu-id="6b7d6-120">字符串</span><span class="sxs-lookup"><span data-stu-id="6b7d6-120">String</span></span>|<span data-ttu-id="6b7d6-121">通知文件的提供程序生成/计算风险分数。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="6b7d6-122">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b7d6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b7d6-123">JSON representation</span></span>

<span data-ttu-id="6b7d6-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b7d6-124">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/filesecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
