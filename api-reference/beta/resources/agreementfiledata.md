---
title: agreementFileData 资源类型
description: 表示 azure Active Directory (azure AD) 使用条款协议文件的 blob。
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544108"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="f9f2a-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9f2a-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f2a-104">表示 azure Active Directory (azure AD) 使用条款协议文件的 blob。</span><span class="sxs-lookup"><span data-stu-id="f9f2a-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="f9f2a-105">属性</span><span class="sxs-lookup"><span data-stu-id="f9f2a-105">Properties</span></span>
| <span data-ttu-id="f9f2a-106">方法</span><span class="sxs-lookup"><span data-stu-id="f9f2a-106">Method</span></span>       | <span data-ttu-id="f9f2a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9f2a-107">Return Type</span></span> | <span data-ttu-id="f9f2a-108">说明</span><span class="sxs-lookup"><span data-stu-id="f9f2a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9f2a-109">data</span><span class="sxs-lookup"><span data-stu-id="f9f2a-109">data</span></span>|<span data-ttu-id="f9f2a-110">Binary</span><span class="sxs-lookup"><span data-stu-id="f9f2a-110">Binary</span></span>|<span data-ttu-id="f9f2a-111">代表使用条款的 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="f9f2a-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="f9f2a-112">只读。</span><span class="sxs-lookup"><span data-stu-id="f9f2a-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9f2a-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9f2a-113">JSON representation</span></span>

<span data-ttu-id="f9f2a-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9f2a-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfiledata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
