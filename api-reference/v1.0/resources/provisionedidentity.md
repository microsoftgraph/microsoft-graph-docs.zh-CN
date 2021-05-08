---
title: provisionedIdentity 资源类型
description: 描述与设置对象摘要事件关联的标识。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 083609787920d840d8576d1c2a7cd5e39945768c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241534"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="a5ad0-103">provisionedIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5ad0-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="a5ad0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5ad0-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="a5ad0-105">描述与设置对象摘要事件关联的标识。</span><span class="sxs-lookup"><span data-stu-id="a5ad0-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="a5ad0-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5ad0-106">Properties</span></span>

| <span data-ttu-id="a5ad0-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5ad0-107">Property</span></span>     | <span data-ttu-id="a5ad0-108">类型</span><span class="sxs-lookup"><span data-stu-id="a5ad0-108">Type</span></span>        | <span data-ttu-id="a5ad0-109">说明</span><span class="sxs-lookup"><span data-stu-id="a5ad0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5ad0-110">详细信息</span><span class="sxs-lookup"><span data-stu-id="a5ad0-110">details</span></span>|[<span data-ttu-id="a5ad0-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="a5ad0-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="a5ad0-112">标识的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5ad0-112">Details of the identity.</span></span>|
|<span data-ttu-id="a5ad0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a5ad0-113">displayName</span></span>|<span data-ttu-id="a5ad0-114">String</span><span class="sxs-lookup"><span data-stu-id="a5ad0-114">String</span></span>|<span data-ttu-id="a5ad0-115">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a5ad0-115">Display name of the identity.</span></span> |
|<span data-ttu-id="a5ad0-116">id</span><span class="sxs-lookup"><span data-stu-id="a5ad0-116">id</span></span>|<span data-ttu-id="a5ad0-117">String</span><span class="sxs-lookup"><span data-stu-id="a5ad0-117">String</span></span>|<span data-ttu-id="a5ad0-118">唯一标识标识。</span><span class="sxs-lookup"><span data-stu-id="a5ad0-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="a5ad0-119">identityType</span><span class="sxs-lookup"><span data-stu-id="a5ad0-119">identityType</span></span>|<span data-ttu-id="a5ad0-120">String</span><span class="sxs-lookup"><span data-stu-id="a5ad0-120">String</span></span>|<span data-ttu-id="a5ad0-121">已预配的标识类型，例如"user"或"group"。</span><span class="sxs-lookup"><span data-stu-id="a5ad0-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5ad0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5ad0-122">JSON representation</span></span>

<span data-ttu-id="a5ad0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5ad0-123">The following is a JSON representation of the resource.</span></span>

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


