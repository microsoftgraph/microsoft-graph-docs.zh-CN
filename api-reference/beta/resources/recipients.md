---
title: 收件人资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 570b740fe5ed19a7308d74cf4710e2772d101e52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521241"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="06092-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="06092-103">recipients resource type</span></span>

<span data-ttu-id="06092-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="06092-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="06092-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06092-105">JSON representation</span></span>

<span data-ttu-id="06092-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06092-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="06092-107">属性</span><span class="sxs-lookup"><span data-stu-id="06092-107">Properties</span></span>
| <span data-ttu-id="06092-108">属性</span><span class="sxs-lookup"><span data-stu-id="06092-108">Property</span></span>     | <span data-ttu-id="06092-109">类型</span><span class="sxs-lookup"><span data-stu-id="06092-109">Type</span></span>   |<span data-ttu-id="06092-110">说明</span><span class="sxs-lookup"><span data-stu-id="06092-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06092-111">alias</span><span class="sxs-lookup"><span data-stu-id="06092-111">alias</span></span>|<span data-ttu-id="06092-112">String</span><span class="sxs-lookup"><span data-stu-id="06092-112">String</span></span>||
|<span data-ttu-id="06092-113">email</span><span class="sxs-lookup"><span data-stu-id="06092-113">email</span></span>|<span data-ttu-id="06092-114">String</span><span class="sxs-lookup"><span data-stu-id="06092-114">String</span></span>||
|<span data-ttu-id="06092-115">objectId</span><span class="sxs-lookup"><span data-stu-id="06092-115">objectId</span></span>|<span data-ttu-id="06092-116">String</span><span class="sxs-lookup"><span data-stu-id="06092-116">String</span></span>||
|<span data-ttu-id="06092-117">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="06092-117">permissionIdentityType</span></span>|<span data-ttu-id="06092-118">String</span><span class="sxs-lookup"><span data-stu-id="06092-118">String</span></span>||

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
