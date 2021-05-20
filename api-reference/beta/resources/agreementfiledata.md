---
title: agreementFileData 资源类型
description: 表示 Azure AD Azure Active Directory (的 blob) 使用条款协议文件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 0531cfd16c42fb7d2a050c8899eea63b8e333f41
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547560"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="a83ee-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="a83ee-103">agreementFileData resource type</span></span>

<span data-ttu-id="a83ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a83ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a83ee-105">表示 Azure AD Azure Active Directory (的 blob) 使用条款协议文件。</span><span class="sxs-lookup"><span data-stu-id="a83ee-105">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="a83ee-106">属性</span><span class="sxs-lookup"><span data-stu-id="a83ee-106">Properties</span></span>
| <span data-ttu-id="a83ee-107">方法</span><span class="sxs-lookup"><span data-stu-id="a83ee-107">Method</span></span>       | <span data-ttu-id="a83ee-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a83ee-108">Return Type</span></span> | <span data-ttu-id="a83ee-109">说明</span><span class="sxs-lookup"><span data-stu-id="a83ee-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a83ee-110">data</span><span class="sxs-lookup"><span data-stu-id="a83ee-110">data</span></span>|<span data-ttu-id="a83ee-111">二进制</span><span class="sxs-lookup"><span data-stu-id="a83ee-111">Binary</span></span>|<span data-ttu-id="a83ee-112">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="a83ee-112">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="a83ee-113">只读。</span><span class="sxs-lookup"><span data-stu-id="a83ee-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a83ee-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a83ee-114">JSON representation</span></span>

<span data-ttu-id="a83ee-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a83ee-115">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


