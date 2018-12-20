---
title: " certificationControl 资源类型"
description: 此资源包含合规性与关联的证书数据安全分数控件。
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380943"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="4dcad-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="4dcad-103">certificationControl resource type</span></span>

<span data-ttu-id="4dcad-104">包含合规性与关联的证书数据安全分数控件。</span><span class="sxs-lookup"><span data-stu-id="4dcad-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="4dcad-105">属性</span><span class="sxs-lookup"><span data-stu-id="4dcad-105">Property</span></span> |<span data-ttu-id="4dcad-106">类型</span><span class="sxs-lookup"><span data-stu-id="4dcad-106">Type</span></span> |<span data-ttu-id="4dcad-107">说明</span><span class="sxs-lookup"><span data-stu-id="4dcad-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="4dcad-108">name</span><span class="sxs-lookup"><span data-stu-id="4dcad-108">name</span></span> | <span data-ttu-id="4dcad-109">string</span><span class="sxs-lookup"><span data-stu-id="4dcad-109">string</span></span> | <span data-ttu-id="4dcad-110">证书控件名称</span><span class="sxs-lookup"><span data-stu-id="4dcad-110">Certification control name</span></span> |
|<span data-ttu-id="4dcad-111">url</span><span class="sxs-lookup"><span data-stu-id="4dcad-111">url</span></span> | <span data-ttu-id="4dcad-112">string</span><span class="sxs-lookup"><span data-stu-id="4dcad-112">string</span></span> | <span data-ttu-id="4dcad-113">Microsoft 服务的 URL 信任门户</span><span class="sxs-lookup"><span data-stu-id="4dcad-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4dcad-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4dcad-114">JSON representation</span></span>

<span data-ttu-id="4dcad-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dcad-115">The following is a JSON representation of the resource.</span></span>

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
