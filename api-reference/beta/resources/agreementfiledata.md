---
title: agreementFileData 资源类型
description: 表示 Azure Active Directory （Azure AD）使用条款协议文件的 blob。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8758de3282bb59220423632be0be9c6e035c18b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508364"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="6efa3-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="6efa3-103">agreementFileData resource type</span></span>

<span data-ttu-id="6efa3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6efa3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6efa3-105">表示 Azure Active Directory （Azure AD）使用条款协议文件的 blob。</span><span class="sxs-lookup"><span data-stu-id="6efa3-105">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="6efa3-106">属性</span><span class="sxs-lookup"><span data-stu-id="6efa3-106">Properties</span></span>
| <span data-ttu-id="6efa3-107">方法</span><span class="sxs-lookup"><span data-stu-id="6efa3-107">Method</span></span>       | <span data-ttu-id="6efa3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6efa3-108">Return Type</span></span> | <span data-ttu-id="6efa3-109">说明</span><span class="sxs-lookup"><span data-stu-id="6efa3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6efa3-110">data</span><span class="sxs-lookup"><span data-stu-id="6efa3-110">data</span></span>|<span data-ttu-id="6efa3-111">Binary</span><span class="sxs-lookup"><span data-stu-id="6efa3-111">Binary</span></span>|<span data-ttu-id="6efa3-112">代表使用条款的 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="6efa3-112">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="6efa3-113">只读。</span><span class="sxs-lookup"><span data-stu-id="6efa3-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6efa3-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6efa3-114">JSON representation</span></span>

<span data-ttu-id="6efa3-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6efa3-115">The following is a JSON representation of the resource.</span></span>

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
