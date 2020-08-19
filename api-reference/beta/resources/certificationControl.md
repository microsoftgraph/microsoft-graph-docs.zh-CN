---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f6ecfa2ffddd362ba6c166d9dc839aedaf6f4723
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810578"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="7728d-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="7728d-103">certificationControl resource type</span></span>

<span data-ttu-id="7728d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7728d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7728d-105">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="7728d-105">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="7728d-106">属性</span><span class="sxs-lookup"><span data-stu-id="7728d-106">Property</span></span> |<span data-ttu-id="7728d-107">类型</span><span class="sxs-lookup"><span data-stu-id="7728d-107">Type</span></span> |<span data-ttu-id="7728d-108">说明</span><span class="sxs-lookup"><span data-stu-id="7728d-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="7728d-109">name</span><span class="sxs-lookup"><span data-stu-id="7728d-109">name</span></span> | <span data-ttu-id="7728d-110">string</span><span class="sxs-lookup"><span data-stu-id="7728d-110">string</span></span> | <span data-ttu-id="7728d-111">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="7728d-111">Certification control name</span></span> |
|<span data-ttu-id="7728d-112">url</span><span class="sxs-lookup"><span data-stu-id="7728d-112">url</span></span> | <span data-ttu-id="7728d-113">string</span><span class="sxs-lookup"><span data-stu-id="7728d-113">string</span></span> | <span data-ttu-id="7728d-114">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="7728d-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7728d-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7728d-115">JSON representation</span></span>

<span data-ttu-id="7728d-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7728d-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
