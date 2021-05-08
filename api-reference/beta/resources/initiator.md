---
title: 发起者资源类型
description: 描述发起预配事件的人或发起者。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f1085b6a9b04ef2ad3cd584ac9e0d4dc6c88f037
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232058"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="aada5-103">发起者资源类型</span><span class="sxs-lookup"><span data-stu-id="aada5-103">initiator resource type</span></span>

<span data-ttu-id="aada5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aada5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aada5-105">描述发起预配事件的人或发起者。</span><span class="sxs-lookup"><span data-stu-id="aada5-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="aada5-106">属性</span><span class="sxs-lookup"><span data-stu-id="aada5-106">Properties</span></span>

| <span data-ttu-id="aada5-107">属性</span><span class="sxs-lookup"><span data-stu-id="aada5-107">Property</span></span>     | <span data-ttu-id="aada5-108">类型</span><span class="sxs-lookup"><span data-stu-id="aada5-108">Type</span></span>        | <span data-ttu-id="aada5-109">说明</span><span class="sxs-lookup"><span data-stu-id="aada5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aada5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="aada5-110">displayName</span></span>|<span data-ttu-id="aada5-111">String</span><span class="sxs-lookup"><span data-stu-id="aada5-111">String</span></span>|<span data-ttu-id="aada5-112">发起预配事件的人员或服务的名称。</span><span class="sxs-lookup"><span data-stu-id="aada5-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="aada5-113">id</span><span class="sxs-lookup"><span data-stu-id="aada5-113">id</span></span>|<span data-ttu-id="aada5-114">String</span><span class="sxs-lookup"><span data-stu-id="aada5-114">String</span></span>|<span data-ttu-id="aada5-115">唯一标识发起预配事件的人员或服务。</span><span class="sxs-lookup"><span data-stu-id="aada5-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="aada5-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="aada5-116">initiatorType</span></span>|<span data-ttu-id="aada5-117">String</span><span class="sxs-lookup"><span data-stu-id="aada5-117">String</span></span>| <span data-ttu-id="aada5-118">发起人的类型。</span><span class="sxs-lookup"><span data-stu-id="aada5-118">Type of initiator.</span></span> <span data-ttu-id="aada5-119">可取值为：`user`、`application`、`system`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="aada5-119">Possible values are: `user`, `application`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aada5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aada5-120">JSON representation</span></span>

<span data-ttu-id="aada5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aada5-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


