---
title: 收件人资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c94bde1d76155a6aa3c2651cfe7106f70e32b78d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008787"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="60d8a-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="60d8a-103">recipients resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="60d8a-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60d8a-104">JSON representation</span></span>

<span data-ttu-id="60d8a-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60d8a-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="60d8a-106">属性</span><span class="sxs-lookup"><span data-stu-id="60d8a-106">Properties</span></span>
| <span data-ttu-id="60d8a-107">属性</span><span class="sxs-lookup"><span data-stu-id="60d8a-107">Property</span></span>     | <span data-ttu-id="60d8a-108">类型</span><span class="sxs-lookup"><span data-stu-id="60d8a-108">Type</span></span>   |<span data-ttu-id="60d8a-109">说明</span><span class="sxs-lookup"><span data-stu-id="60d8a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60d8a-110">alias</span><span class="sxs-lookup"><span data-stu-id="60d8a-110">alias</span></span>|<span data-ttu-id="60d8a-111">String</span><span class="sxs-lookup"><span data-stu-id="60d8a-111">String</span></span>||
|<span data-ttu-id="60d8a-112">email</span><span class="sxs-lookup"><span data-stu-id="60d8a-112">email</span></span>|<span data-ttu-id="60d8a-113">String</span><span class="sxs-lookup"><span data-stu-id="60d8a-113">String</span></span>||
|<span data-ttu-id="60d8a-114">objectId</span><span class="sxs-lookup"><span data-stu-id="60d8a-114">objectId</span></span>|<span data-ttu-id="60d8a-115">String</span><span class="sxs-lookup"><span data-stu-id="60d8a-115">String</span></span>||
|<span data-ttu-id="60d8a-116">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="60d8a-116">permissionIdentityType</span></span>|<span data-ttu-id="60d8a-117">String</span><span class="sxs-lookup"><span data-stu-id="60d8a-117">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
