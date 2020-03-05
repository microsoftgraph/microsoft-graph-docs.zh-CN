---
title: provisionedIdentity 资源类型
description: 描述与设置对象摘要事件关联的标识。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86363bdf77f83e6903c86362c2797c51d1215073
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521353"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="2c536-103">provisionedIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c536-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="2c536-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2c536-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c536-105">描述与设置对象摘要事件关联的标识。</span><span class="sxs-lookup"><span data-stu-id="2c536-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="2c536-106">属性</span><span class="sxs-lookup"><span data-stu-id="2c536-106">Properties</span></span>

| <span data-ttu-id="2c536-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c536-107">Property</span></span>     | <span data-ttu-id="2c536-108">类型</span><span class="sxs-lookup"><span data-stu-id="2c536-108">Type</span></span>        | <span data-ttu-id="2c536-109">说明</span><span class="sxs-lookup"><span data-stu-id="2c536-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c536-110">详细信息</span><span class="sxs-lookup"><span data-stu-id="2c536-110">details</span></span>|[<span data-ttu-id="2c536-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="2c536-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="2c536-112">标识的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c536-112">Details of the identity.</span></span>|
|<span data-ttu-id="2c536-113">displayName</span><span class="sxs-lookup"><span data-stu-id="2c536-113">displayName</span></span>|<span data-ttu-id="2c536-114">String</span><span class="sxs-lookup"><span data-stu-id="2c536-114">String</span></span>|<span data-ttu-id="2c536-115">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2c536-115">Display name of the identity.</span></span> |
|<span data-ttu-id="2c536-116">id</span><span class="sxs-lookup"><span data-stu-id="2c536-116">id</span></span>|<span data-ttu-id="2c536-117">String</span><span class="sxs-lookup"><span data-stu-id="2c536-117">String</span></span>|<span data-ttu-id="2c536-118">唯一标识标识。</span><span class="sxs-lookup"><span data-stu-id="2c536-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="2c536-119">identityType</span><span class="sxs-lookup"><span data-stu-id="2c536-119">identityType</span></span>|<span data-ttu-id="2c536-120">String</span><span class="sxs-lookup"><span data-stu-id="2c536-120">String</span></span>|<span data-ttu-id="2c536-121">已设置的标识类型，如 "user" 或 "group"。</span><span class="sxs-lookup"><span data-stu-id="2c536-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c536-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c536-122">JSON representation</span></span>

<span data-ttu-id="2c536-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c536-123">The following is a JSON representation of the resource.</span></span>

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
