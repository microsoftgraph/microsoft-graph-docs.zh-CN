---
title: 发起程序资源类型
description: 描述启动设置事件的目标或内容。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2846c247d4a0d196d4c620f447b40d47cd486c81
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349358"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="2c68d-103">发起程序资源类型</span><span class="sxs-lookup"><span data-stu-id="2c68d-103">initiator resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c68d-104">描述启动设置事件的目标或内容。</span><span class="sxs-lookup"><span data-stu-id="2c68d-104">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="2c68d-105">属性</span><span class="sxs-lookup"><span data-stu-id="2c68d-105">Properties</span></span>

| <span data-ttu-id="2c68d-106">属性</span><span class="sxs-lookup"><span data-stu-id="2c68d-106">Property</span></span>     | <span data-ttu-id="2c68d-107">类型</span><span class="sxs-lookup"><span data-stu-id="2c68d-107">Type</span></span>        | <span data-ttu-id="2c68d-108">说明</span><span class="sxs-lookup"><span data-stu-id="2c68d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c68d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="2c68d-109">displayName</span></span>|<span data-ttu-id="2c68d-110">String</span><span class="sxs-lookup"><span data-stu-id="2c68d-110">String</span></span>|<span data-ttu-id="2c68d-111">启动设置事件的人员或服务的名称。</span><span class="sxs-lookup"><span data-stu-id="2c68d-111">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="2c68d-112">id</span><span class="sxs-lookup"><span data-stu-id="2c68d-112">id</span></span>|<span data-ttu-id="2c68d-113">String</span><span class="sxs-lookup"><span data-stu-id="2c68d-113">String</span></span>|<span data-ttu-id="2c68d-114">唯一标识启动设置事件的人员或服务。</span><span class="sxs-lookup"><span data-stu-id="2c68d-114">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="2c68d-115">initiatorType</span><span class="sxs-lookup"><span data-stu-id="2c68d-115">initiatorType</span></span>|<span data-ttu-id="2c68d-116">String</span><span class="sxs-lookup"><span data-stu-id="2c68d-116">String</span></span>| <span data-ttu-id="2c68d-117">发起程序的类型。</span><span class="sxs-lookup"><span data-stu-id="2c68d-117">Type of initiator.</span></span> <span data-ttu-id="2c68d-118">可取值为：`user`、`app`、`system`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c68d-118">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c68d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c68d-119">JSON representation</span></span>

<span data-ttu-id="2c68d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c68d-120">The following is a JSON representation of the resource.</span></span>

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
