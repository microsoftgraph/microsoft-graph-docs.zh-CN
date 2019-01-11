---
title: agreementFileData 资源类型
description: 代表 Azure Active Directory 的 blob (Azure AD) 使用条款使用协议文件。
localization_priority: Normal
ms.openlocfilehash: 64de3a72ad648225f24429987f5729f76ed8a2e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815215"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="a87e1-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="a87e1-103">agreementFileData resource type</span></span>

> <span data-ttu-id="a87e1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a87e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a87e1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a87e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a87e1-106">代表 Azure Active Directory 的 blob (Azure AD) 使用条款使用协议文件。</span><span class="sxs-lookup"><span data-stu-id="a87e1-106">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="a87e1-107">属性</span><span class="sxs-lookup"><span data-stu-id="a87e1-107">Properties</span></span>
| <span data-ttu-id="a87e1-108">方法</span><span class="sxs-lookup"><span data-stu-id="a87e1-108">Method</span></span>       | <span data-ttu-id="a87e1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a87e1-109">Return Type</span></span> | <span data-ttu-id="a87e1-110">说明</span><span class="sxs-lookup"><span data-stu-id="a87e1-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a87e1-111">data</span><span class="sxs-lookup"><span data-stu-id="a87e1-111">data</span></span>|<span data-ttu-id="a87e1-112">Binary</span><span class="sxs-lookup"><span data-stu-id="a87e1-112">Binary</span></span>|<span data-ttu-id="a87e1-113">表示使用 PDF 文档中的条款的数据。</span><span class="sxs-lookup"><span data-stu-id="a87e1-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="a87e1-114">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a87e1-114">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a87e1-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a87e1-115">JSON representation</span></span>

<span data-ttu-id="a87e1-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a87e1-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
