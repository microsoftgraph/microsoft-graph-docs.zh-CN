---
title: 发起者资源类型
description: 描述设置事件发起人或发起者。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2aa8c3f365402569d7a9987d9152bae5e4e3c580
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130241"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="b8e93-103">发起者资源类型</span><span class="sxs-lookup"><span data-stu-id="b8e93-103">initiator resource type</span></span>

<span data-ttu-id="b8e93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8e93-105">描述设置事件发起人或发起者。</span><span class="sxs-lookup"><span data-stu-id="b8e93-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="b8e93-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8e93-106">Properties</span></span>

| <span data-ttu-id="b8e93-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8e93-107">Property</span></span>     | <span data-ttu-id="b8e93-108">类型</span><span class="sxs-lookup"><span data-stu-id="b8e93-108">Type</span></span>        | <span data-ttu-id="b8e93-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8e93-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8e93-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b8e93-110">displayName</span></span>|<span data-ttu-id="b8e93-111">字符串</span><span class="sxs-lookup"><span data-stu-id="b8e93-111">String</span></span>|<span data-ttu-id="b8e93-112">发起预配事件的人员或服务的名称。</span><span class="sxs-lookup"><span data-stu-id="b8e93-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="b8e93-113">id</span><span class="sxs-lookup"><span data-stu-id="b8e93-113">id</span></span>|<span data-ttu-id="b8e93-114">字符串</span><span class="sxs-lookup"><span data-stu-id="b8e93-114">String</span></span>|<span data-ttu-id="b8e93-115">唯一标识发起预配事件的人员或服务。</span><span class="sxs-lookup"><span data-stu-id="b8e93-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="b8e93-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="b8e93-116">initiatorType</span></span>|<span data-ttu-id="b8e93-117">字符串</span><span class="sxs-lookup"><span data-stu-id="b8e93-117">String</span></span>| <span data-ttu-id="b8e93-118">发起人的类型。</span><span class="sxs-lookup"><span data-stu-id="b8e93-118">Type of initiator.</span></span> <span data-ttu-id="b8e93-119">可取值为：`user`、`app`、`system`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b8e93-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8e93-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8e93-120">JSON representation</span></span>

<span data-ttu-id="b8e93-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8e93-121">The following is a JSON representation of the resource.</span></span>

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


