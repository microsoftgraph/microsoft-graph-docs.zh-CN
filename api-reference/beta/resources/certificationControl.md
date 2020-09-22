---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4f2be439f1b286a8d916fe80a7b4fcb4f6d60071
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016819"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="d358a-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="d358a-103">certificationControl resource type</span></span>

<span data-ttu-id="d358a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d358a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d358a-105">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="d358a-105">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="d358a-106">属性</span><span class="sxs-lookup"><span data-stu-id="d358a-106">Property</span></span> |<span data-ttu-id="d358a-107">类型</span><span class="sxs-lookup"><span data-stu-id="d358a-107">Type</span></span> |<span data-ttu-id="d358a-108">说明</span><span class="sxs-lookup"><span data-stu-id="d358a-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d358a-109">name</span><span class="sxs-lookup"><span data-stu-id="d358a-109">name</span></span> | <span data-ttu-id="d358a-110">string</span><span class="sxs-lookup"><span data-stu-id="d358a-110">string</span></span> | <span data-ttu-id="d358a-111">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="d358a-111">Certification control name</span></span> |
|<span data-ttu-id="d358a-112">url</span><span class="sxs-lookup"><span data-stu-id="d358a-112">url</span></span> | <span data-ttu-id="d358a-113">string</span><span class="sxs-lookup"><span data-stu-id="d358a-113">string</span></span> | <span data-ttu-id="d358a-114">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="d358a-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d358a-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d358a-115">JSON representation</span></span>

<span data-ttu-id="d358a-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d358a-116">The following is a JSON representation of the resource.</span></span>

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


