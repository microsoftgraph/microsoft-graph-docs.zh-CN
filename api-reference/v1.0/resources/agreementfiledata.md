---
title: agreementFileData 资源类型
description: 表示 Azure AD (Azure AD) Azure Active Directory 协议文件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 31837b69a87f731f41de23a458dedec665bfe5c4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722613"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="a36f8-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="a36f8-103">agreementFileData resource type</span></span>

<span data-ttu-id="a36f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a36f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a36f8-105">表示 Azure AD (Azure AD) Azure Active Directory 协议文件。</span><span class="sxs-lookup"><span data-stu-id="a36f8-105">Represents an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="a36f8-106">属性</span><span class="sxs-lookup"><span data-stu-id="a36f8-106">Properties</span></span>
| <span data-ttu-id="a36f8-107">方法</span><span class="sxs-lookup"><span data-stu-id="a36f8-107">Method</span></span>       | <span data-ttu-id="a36f8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a36f8-108">Return Type</span></span> | <span data-ttu-id="a36f8-109">说明</span><span class="sxs-lookup"><span data-stu-id="a36f8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a36f8-110">data</span><span class="sxs-lookup"><span data-stu-id="a36f8-110">data</span></span>|<span data-ttu-id="a36f8-111">Binary</span><span class="sxs-lookup"><span data-stu-id="a36f8-111">Binary</span></span>|<span data-ttu-id="a36f8-112">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="a36f8-112">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="a36f8-113">只读。</span><span class="sxs-lookup"><span data-stu-id="a36f8-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a36f8-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a36f8-114">JSON representation</span></span>

<span data-ttu-id="a36f8-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a36f8-115">The following is a JSON representation of the resource.</span></span>

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


