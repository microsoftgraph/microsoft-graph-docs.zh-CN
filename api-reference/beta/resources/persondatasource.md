---
title: personDataSource 资源类型
description: 代表用户数据来自，例如目录和 Outlook 联系人的源。
ms.openlocfilehash: 1c5aeb2cbb36398eb3c7184550235fc7194f5e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043653"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="ae807-103">personDataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae807-103">personDataSource resource type</span></span>

> <span data-ttu-id="ae807-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae807-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae807-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae807-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae807-106">代表用户数据来自，例如目录和 Outlook 联系人的源。</span><span class="sxs-lookup"><span data-stu-id="ae807-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae807-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae807-107">JSON representation</span></span>

<span data-ttu-id="ae807-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae807-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="ae807-109">属性</span><span class="sxs-lookup"><span data-stu-id="ae807-109">Properties</span></span>
| <span data-ttu-id="ae807-110">属性</span><span class="sxs-lookup"><span data-stu-id="ae807-110">Property</span></span>     | <span data-ttu-id="ae807-111">类型</span><span class="sxs-lookup"><span data-stu-id="ae807-111">Type</span></span>   |<span data-ttu-id="ae807-112">说明</span><span class="sxs-lookup"><span data-stu-id="ae807-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae807-113">type</span><span class="sxs-lookup"><span data-stu-id="ae807-113">type</span></span>|<span data-ttu-id="ae807-114">字符串</span><span class="sxs-lookup"><span data-stu-id="ae807-114">String</span></span>|<span data-ttu-id="ae807-115">数据源的类型。</span><span class="sxs-lookup"><span data-stu-id="ae807-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->