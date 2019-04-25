---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535411"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="4f9d7-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f9d7-103">certificationControl resource type</span></span>

<span data-ttu-id="4f9d7-104">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="4f9d7-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="4f9d7-105">属性</span><span class="sxs-lookup"><span data-stu-id="4f9d7-105">Property</span></span> |<span data-ttu-id="4f9d7-106">类型</span><span class="sxs-lookup"><span data-stu-id="4f9d7-106">Type</span></span> |<span data-ttu-id="4f9d7-107">说明</span><span class="sxs-lookup"><span data-stu-id="4f9d7-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="4f9d7-108">name</span><span class="sxs-lookup"><span data-stu-id="4f9d7-108">name</span></span> | <span data-ttu-id="4f9d7-109">string</span><span class="sxs-lookup"><span data-stu-id="4f9d7-109">string</span></span> | <span data-ttu-id="4f9d7-110">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="4f9d7-110">Certification control name</span></span> |
|<span data-ttu-id="4f9d7-111">url</span><span class="sxs-lookup"><span data-stu-id="4f9d7-111">url</span></span> | <span data-ttu-id="4f9d7-112">string</span><span class="sxs-lookup"><span data-stu-id="4f9d7-112">string</span></span> | <span data-ttu-id="4f9d7-113">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="4f9d7-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f9d7-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f9d7-114">JSON representation</span></span>

<span data-ttu-id="4f9d7-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f9d7-115">The following is a JSON representation of the resource.</span></span>

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
