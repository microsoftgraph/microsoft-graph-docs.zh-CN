---
title: 发起程序资源类型
description: 描述启动设置事件的目标或内容。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6d279ce00855cb8125085e48bddf63f1b8f0e5e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461725"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="00373-103">发起程序资源类型</span><span class="sxs-lookup"><span data-stu-id="00373-103">initiator resource type</span></span>

<span data-ttu-id="00373-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00373-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00373-105">描述启动设置事件的目标或内容。</span><span class="sxs-lookup"><span data-stu-id="00373-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="00373-106">属性</span><span class="sxs-lookup"><span data-stu-id="00373-106">Properties</span></span>

| <span data-ttu-id="00373-107">属性</span><span class="sxs-lookup"><span data-stu-id="00373-107">Property</span></span>     | <span data-ttu-id="00373-108">类型</span><span class="sxs-lookup"><span data-stu-id="00373-108">Type</span></span>        | <span data-ttu-id="00373-109">说明</span><span class="sxs-lookup"><span data-stu-id="00373-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00373-110">displayName</span><span class="sxs-lookup"><span data-stu-id="00373-110">displayName</span></span>|<span data-ttu-id="00373-111">String</span><span class="sxs-lookup"><span data-stu-id="00373-111">String</span></span>|<span data-ttu-id="00373-112">启动设置事件的人员或服务的名称。</span><span class="sxs-lookup"><span data-stu-id="00373-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="00373-113">id</span><span class="sxs-lookup"><span data-stu-id="00373-113">id</span></span>|<span data-ttu-id="00373-114">String</span><span class="sxs-lookup"><span data-stu-id="00373-114">String</span></span>|<span data-ttu-id="00373-115">唯一标识启动设置事件的人员或服务。</span><span class="sxs-lookup"><span data-stu-id="00373-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="00373-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="00373-116">initiatorType</span></span>|<span data-ttu-id="00373-117">String</span><span class="sxs-lookup"><span data-stu-id="00373-117">String</span></span>| <span data-ttu-id="00373-118">发起程序的类型。</span><span class="sxs-lookup"><span data-stu-id="00373-118">Type of initiator.</span></span> <span data-ttu-id="00373-119">可取值为：`user`、`app`、`system`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="00373-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00373-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00373-120">JSON representation</span></span>

<span data-ttu-id="00373-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00373-121">The following is a JSON representation of the resource.</span></span>

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
