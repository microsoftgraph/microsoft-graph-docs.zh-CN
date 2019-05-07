---
title: certificationControl 资源类型
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: c92d129b6849898abe7202b9c2f539f26d2e1ebe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629311"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="fb823-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb823-103">certificationControl resource type</span></span>

<span data-ttu-id="fb823-104">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="fb823-104">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="fb823-105">属性</span><span class="sxs-lookup"><span data-stu-id="fb823-105">Properties</span></span>

|<span data-ttu-id="fb823-106">属性</span><span class="sxs-lookup"><span data-stu-id="fb823-106">Property</span></span> |<span data-ttu-id="fb823-107">类型</span><span class="sxs-lookup"><span data-stu-id="fb823-107">Type</span></span> |<span data-ttu-id="fb823-108">说明</span><span class="sxs-lookup"><span data-stu-id="fb823-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="fb823-109">name</span><span class="sxs-lookup"><span data-stu-id="fb823-109">name</span></span>|<span data-ttu-id="fb823-110">字符串</span><span class="sxs-lookup"><span data-stu-id="fb823-110">String</span></span>|<span data-ttu-id="fb823-111">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="fb823-111">Certification control name</span></span> |
|<span data-ttu-id="fb823-112">url</span><span class="sxs-lookup"><span data-stu-id="fb823-112">url</span></span>|<span data-ttu-id="fb823-113">String</span><span class="sxs-lookup"><span data-stu-id="fb823-113">String</span></span>|<span data-ttu-id="fb823-114">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="fb823-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb823-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb823-115">JSON representation</span></span>

<span data-ttu-id="fb823-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb823-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
