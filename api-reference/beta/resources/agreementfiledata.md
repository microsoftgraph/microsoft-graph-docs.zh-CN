---
title: agreementFileData 资源类型
description: 代表 Azure Active Directory 的 blob (Azure AD) 使用条款使用协议文件。
ms.openlocfilehash: 557725e14f4954f8b2c10112e1013beb71dda0be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045396"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="6fe95-103">agreementFileData 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fe95-103">agreementFileData resource type</span></span>

> <span data-ttu-id="6fe95-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6fe95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fe95-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6fe95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6fe95-106">代表 Azure Active Directory 的 blob (Azure AD) 使用条款使用协议文件。</span><span class="sxs-lookup"><span data-stu-id="6fe95-106">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="6fe95-107">属性</span><span class="sxs-lookup"><span data-stu-id="6fe95-107">Properties</span></span>
| <span data-ttu-id="6fe95-108">方法</span><span class="sxs-lookup"><span data-stu-id="6fe95-108">Method</span></span>       | <span data-ttu-id="6fe95-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fe95-109">Return Type</span></span> | <span data-ttu-id="6fe95-110">说明</span><span class="sxs-lookup"><span data-stu-id="6fe95-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fe95-111">data</span><span class="sxs-lookup"><span data-stu-id="6fe95-111">data</span></span>|<span data-ttu-id="6fe95-112">二进制数</span><span class="sxs-lookup"><span data-stu-id="6fe95-112">Binary</span></span>|<span data-ttu-id="6fe95-113">表示使用 PDF 文档中的条款的数据。</span><span class="sxs-lookup"><span data-stu-id="6fe95-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="6fe95-114">只读。</span><span class="sxs-lookup"><span data-stu-id="6fe95-114">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fe95-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fe95-115">JSON representation</span></span>

<span data-ttu-id="6fe95-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fe95-116">The following is a JSON representation of the resource.</span></span>

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
