---
title: fileSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526954"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="1a5f0-104">fileSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a5f0-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a5f0-105">包含与通知相关的文件 （处理） 有关的信息。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="1a5f0-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a5f0-106">Properties</span></span>

| <span data-ttu-id="1a5f0-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a5f0-107">Property</span></span>   | <span data-ttu-id="1a5f0-108">类型</span><span class="sxs-lookup"><span data-stu-id="1a5f0-108">Type</span></span>|<span data-ttu-id="1a5f0-109">说明</span><span class="sxs-lookup"><span data-stu-id="1a5f0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a5f0-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="1a5f0-110">fileHash</span></span>|[<span data-ttu-id="1a5f0-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="1a5f0-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="1a5f0-112">包含文件哈希 （加密和位置） 的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="1a5f0-113">name</span><span class="sxs-lookup"><span data-stu-id="1a5f0-113">name</span></span>|<span data-ttu-id="1a5f0-114">字符串</span><span class="sxs-lookup"><span data-stu-id="1a5f0-114">String</span></span>|<span data-ttu-id="1a5f0-115">文件名 （不带路径）。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-115">File name (without path).</span></span>|
|<span data-ttu-id="1a5f0-116">路径</span><span class="sxs-lookup"><span data-stu-id="1a5f0-116">path</span></span>|<span data-ttu-id="1a5f0-117">String</span><span class="sxs-lookup"><span data-stu-id="1a5f0-117">String</span></span>|<span data-ttu-id="1a5f0-118">文件/imageFile 完整文件路径。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="1a5f0-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="1a5f0-119">riskScore</span></span>|<span data-ttu-id="1a5f0-120">String</span><span class="sxs-lookup"><span data-stu-id="1a5f0-120">String</span></span>|<span data-ttu-id="1a5f0-121">提供程序生成/计算风险评分的警报的文件。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="1a5f0-122">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a5f0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a5f0-123">JSON representation</span></span>

<span data-ttu-id="1a5f0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a5f0-124">The following is a JSON representation of the resource.</span></span>

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
