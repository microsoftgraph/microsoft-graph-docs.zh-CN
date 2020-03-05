---
title: synchronizationError 资源类型
description: 表示同步过程中发生的错误。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a754b03379d1e40ba7310283a0efdd94ff30631
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520077"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="30054-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="30054-103">synchronizationError resource type</span></span>

<span data-ttu-id="30054-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="30054-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30054-105">表示同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="30054-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="30054-106">属性</span><span class="sxs-lookup"><span data-stu-id="30054-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="30054-107">属性</span><span class="sxs-lookup"><span data-stu-id="30054-107">Property</span></span>     | <span data-ttu-id="30054-108">类型</span><span class="sxs-lookup"><span data-stu-id="30054-108">Type</span></span>   |<span data-ttu-id="30054-109">说明</span><span class="sxs-lookup"><span data-stu-id="30054-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30054-110">code</span><span class="sxs-lookup"><span data-stu-id="30054-110">code</span></span>|<span data-ttu-id="30054-111">String</span><span class="sxs-lookup"><span data-stu-id="30054-111">String</span></span>||
|<span data-ttu-id="30054-112">message</span><span class="sxs-lookup"><span data-stu-id="30054-112">message</span></span>|<span data-ttu-id="30054-113">String</span><span class="sxs-lookup"><span data-stu-id="30054-113">String</span></span>||
|<span data-ttu-id="30054-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="30054-114">tenantActionable</span></span>|<span data-ttu-id="30054-115">布尔</span><span class="sxs-lookup"><span data-stu-id="30054-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="30054-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30054-116">JSON representation</span></span>

<span data-ttu-id="30054-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30054-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
