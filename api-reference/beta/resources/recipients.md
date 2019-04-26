---
title: 收件人资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 367b796f46dce0f68e8077f7eba93ef0216279f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343953"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="6ef2e-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="6ef2e-103">recipients resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="6ef2e-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ef2e-104">JSON representation</span></span>

<span data-ttu-id="6ef2e-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ef2e-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6ef2e-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ef2e-106">Properties</span></span>
| <span data-ttu-id="6ef2e-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ef2e-107">Property</span></span>     | <span data-ttu-id="6ef2e-108">类型</span><span class="sxs-lookup"><span data-stu-id="6ef2e-108">Type</span></span>   |<span data-ttu-id="6ef2e-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ef2e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ef2e-110">alias</span><span class="sxs-lookup"><span data-stu-id="6ef2e-110">alias</span></span>|<span data-ttu-id="6ef2e-111">String</span><span class="sxs-lookup"><span data-stu-id="6ef2e-111">String</span></span>||
|<span data-ttu-id="6ef2e-112">email</span><span class="sxs-lookup"><span data-stu-id="6ef2e-112">email</span></span>|<span data-ttu-id="6ef2e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="6ef2e-113">String</span></span>||
|<span data-ttu-id="6ef2e-114">objectId</span><span class="sxs-lookup"><span data-stu-id="6ef2e-114">objectId</span></span>|<span data-ttu-id="6ef2e-115">String</span><span class="sxs-lookup"><span data-stu-id="6ef2e-115">String</span></span>||
|<span data-ttu-id="6ef2e-116">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="6ef2e-116">permissionIdentityType</span></span>|<span data-ttu-id="6ef2e-117">String</span><span class="sxs-lookup"><span data-stu-id="6ef2e-117">String</span></span>||

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
