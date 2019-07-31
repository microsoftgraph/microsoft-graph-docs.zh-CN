---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 22dc12070a801988d814ba73c6bffe1414bb5218
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012994"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="1fb0c-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fb0c-103">certificationControl resource type</span></span>

<span data-ttu-id="1fb0c-104">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="1fb0c-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="1fb0c-105">属性</span><span class="sxs-lookup"><span data-stu-id="1fb0c-105">Property</span></span> |<span data-ttu-id="1fb0c-106">类型</span><span class="sxs-lookup"><span data-stu-id="1fb0c-106">Type</span></span> |<span data-ttu-id="1fb0c-107">说明</span><span class="sxs-lookup"><span data-stu-id="1fb0c-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="1fb0c-108">name</span><span class="sxs-lookup"><span data-stu-id="1fb0c-108">name</span></span> | <span data-ttu-id="1fb0c-109">string</span><span class="sxs-lookup"><span data-stu-id="1fb0c-109">string</span></span> | <span data-ttu-id="1fb0c-110">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="1fb0c-110">Certification control name</span></span> |
|<span data-ttu-id="1fb0c-111">url</span><span class="sxs-lookup"><span data-stu-id="1fb0c-111">url</span></span> | <span data-ttu-id="1fb0c-112">string</span><span class="sxs-lookup"><span data-stu-id="1fb0c-112">string</span></span> | <span data-ttu-id="1fb0c-113">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="1fb0c-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1fb0c-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fb0c-114">JSON representation</span></span>

<span data-ttu-id="1fb0c-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fb0c-115">The following is a JSON representation of the resource.</span></span>

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
