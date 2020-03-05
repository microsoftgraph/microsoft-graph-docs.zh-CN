---
title: 发起程序资源类型
description: 描述启动设置事件的目标或内容。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 909849775e5bf35c9a29902efbbc3975177956d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496010"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="931f2-103">发起程序资源类型</span><span class="sxs-lookup"><span data-stu-id="931f2-103">initiator resource type</span></span>

<span data-ttu-id="931f2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="931f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="931f2-105">描述启动设置事件的目标或内容。</span><span class="sxs-lookup"><span data-stu-id="931f2-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="931f2-106">属性</span><span class="sxs-lookup"><span data-stu-id="931f2-106">Properties</span></span>

| <span data-ttu-id="931f2-107">属性</span><span class="sxs-lookup"><span data-stu-id="931f2-107">Property</span></span>     | <span data-ttu-id="931f2-108">类型</span><span class="sxs-lookup"><span data-stu-id="931f2-108">Type</span></span>        | <span data-ttu-id="931f2-109">说明</span><span class="sxs-lookup"><span data-stu-id="931f2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="931f2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="931f2-110">displayName</span></span>|<span data-ttu-id="931f2-111">String</span><span class="sxs-lookup"><span data-stu-id="931f2-111">String</span></span>|<span data-ttu-id="931f2-112">启动设置事件的人员或服务的名称。</span><span class="sxs-lookup"><span data-stu-id="931f2-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="931f2-113">id</span><span class="sxs-lookup"><span data-stu-id="931f2-113">id</span></span>|<span data-ttu-id="931f2-114">String</span><span class="sxs-lookup"><span data-stu-id="931f2-114">String</span></span>|<span data-ttu-id="931f2-115">唯一标识启动设置事件的人员或服务。</span><span class="sxs-lookup"><span data-stu-id="931f2-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="931f2-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="931f2-116">initiatorType</span></span>|<span data-ttu-id="931f2-117">String</span><span class="sxs-lookup"><span data-stu-id="931f2-117">String</span></span>| <span data-ttu-id="931f2-118">发起程序的类型。</span><span class="sxs-lookup"><span data-stu-id="931f2-118">Type of initiator.</span></span> <span data-ttu-id="931f2-119">可取值为：`user`、`app`、`system`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="931f2-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="931f2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="931f2-120">JSON representation</span></span>

<span data-ttu-id="931f2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="931f2-121">The following is a JSON representation of the resource.</span></span>

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
