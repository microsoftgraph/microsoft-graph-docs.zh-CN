---
title: certificationControl 资源类型
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ad7c07d269f9dc627de41db621e4d73f0d2c10b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029902"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="83cdd-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="83cdd-103">certificationControl resource type</span></span>

<span data-ttu-id="83cdd-104">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="83cdd-104">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="83cdd-105">属性</span><span class="sxs-lookup"><span data-stu-id="83cdd-105">Properties</span></span>

|<span data-ttu-id="83cdd-106">属性</span><span class="sxs-lookup"><span data-stu-id="83cdd-106">Property</span></span> |<span data-ttu-id="83cdd-107">类型</span><span class="sxs-lookup"><span data-stu-id="83cdd-107">Type</span></span> |<span data-ttu-id="83cdd-108">说明</span><span class="sxs-lookup"><span data-stu-id="83cdd-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="83cdd-109">name</span><span class="sxs-lookup"><span data-stu-id="83cdd-109">name</span></span>|<span data-ttu-id="83cdd-110">String</span><span class="sxs-lookup"><span data-stu-id="83cdd-110">String</span></span>|<span data-ttu-id="83cdd-111">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="83cdd-111">Certification control name</span></span> |
|<span data-ttu-id="83cdd-112">url</span><span class="sxs-lookup"><span data-stu-id="83cdd-112">url</span></span>|<span data-ttu-id="83cdd-113">String</span><span class="sxs-lookup"><span data-stu-id="83cdd-113">String</span></span>|<span data-ttu-id="83cdd-114">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="83cdd-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83cdd-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83cdd-115">JSON representation</span></span>

<span data-ttu-id="83cdd-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83cdd-116">The following is a JSON representation of the resource.</span></span>

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
