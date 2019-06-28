---
title: provisionedIdentity 资源类型
description: 描述与设置对象摘要事件关联的标识。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb535bbba827f93b597c5e41efb128f2ad610ef2
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349339"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="3f9b6-103">provisionedIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f9b6-103">provisionedIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f9b6-104">描述与设置对象摘要事件关联的标识。</span><span class="sxs-lookup"><span data-stu-id="3f9b6-104">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="3f9b6-105">属性</span><span class="sxs-lookup"><span data-stu-id="3f9b6-105">Properties</span></span>

| <span data-ttu-id="3f9b6-106">属性</span><span class="sxs-lookup"><span data-stu-id="3f9b6-106">Property</span></span>     | <span data-ttu-id="3f9b6-107">类型</span><span class="sxs-lookup"><span data-stu-id="3f9b6-107">Type</span></span>        | <span data-ttu-id="3f9b6-108">说明</span><span class="sxs-lookup"><span data-stu-id="3f9b6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3f9b6-109">详细信息</span><span class="sxs-lookup"><span data-stu-id="3f9b6-109">details</span></span>|[<span data-ttu-id="3f9b6-110">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="3f9b6-110">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="3f9b6-111">标识的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3f9b6-111">Details of the identity.</span></span>|
|<span data-ttu-id="3f9b6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3f9b6-112">displayName</span></span>|<span data-ttu-id="3f9b6-113">String</span><span class="sxs-lookup"><span data-stu-id="3f9b6-113">String</span></span>|<span data-ttu-id="3f9b6-114">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3f9b6-114">Display name of the identity.</span></span> |
|<span data-ttu-id="3f9b6-115">id</span><span class="sxs-lookup"><span data-stu-id="3f9b6-115">id</span></span>|<span data-ttu-id="3f9b6-116">String</span><span class="sxs-lookup"><span data-stu-id="3f9b6-116">String</span></span>|<span data-ttu-id="3f9b6-117">唯一标识标识。</span><span class="sxs-lookup"><span data-stu-id="3f9b6-117">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="3f9b6-118">identityType</span><span class="sxs-lookup"><span data-stu-id="3f9b6-118">identityType</span></span>|<span data-ttu-id="3f9b6-119">String</span><span class="sxs-lookup"><span data-stu-id="3f9b6-119">String</span></span>|<span data-ttu-id="3f9b6-120">已设置的标识类型, 如 "user" 或 "group"。</span><span class="sxs-lookup"><span data-stu-id="3f9b6-120">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f9b6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f9b6-121">JSON representation</span></span>

<span data-ttu-id="3f9b6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f9b6-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
