---
title: agreementFileData 资源类型
description: 表示 Azure Active Directory (Azure AD) 使用条款协议文件的 blob。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: da4e600480e6ddd65112323b22f7a905b3ba29db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013421"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="a75ea-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="a75ea-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a75ea-104">表示 Azure Active Directory (Azure AD) 使用条款协议文件的 blob。</span><span class="sxs-lookup"><span data-stu-id="a75ea-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="a75ea-105">属性</span><span class="sxs-lookup"><span data-stu-id="a75ea-105">Properties</span></span>
| <span data-ttu-id="a75ea-106">方法</span><span class="sxs-lookup"><span data-stu-id="a75ea-106">Method</span></span>       | <span data-ttu-id="a75ea-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a75ea-107">Return Type</span></span> | <span data-ttu-id="a75ea-108">说明</span><span class="sxs-lookup"><span data-stu-id="a75ea-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a75ea-109">data</span><span class="sxs-lookup"><span data-stu-id="a75ea-109">data</span></span>|<span data-ttu-id="a75ea-110">Binary</span><span class="sxs-lookup"><span data-stu-id="a75ea-110">Binary</span></span>|<span data-ttu-id="a75ea-111">代表使用条款的 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="a75ea-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="a75ea-112">只读。</span><span class="sxs-lookup"><span data-stu-id="a75ea-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a75ea-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a75ea-113">JSON representation</span></span>

<span data-ttu-id="a75ea-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a75ea-114">The following is a JSON representation of the resource.</span></span>

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
