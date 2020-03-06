---
title: certificationControl 资源类型
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eb792c5ce3b462fa5d2febcd1fb5ed0509d3ef30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531940"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="050ef-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="050ef-103">certificationControl resource type</span></span>

<span data-ttu-id="050ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="050ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="050ef-105">包含与安全得分控制相关联的合规性认证数据。</span><span class="sxs-lookup"><span data-stu-id="050ef-105">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="050ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="050ef-106">Properties</span></span>

|<span data-ttu-id="050ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="050ef-107">Property</span></span> |<span data-ttu-id="050ef-108">类型</span><span class="sxs-lookup"><span data-stu-id="050ef-108">Type</span></span> |<span data-ttu-id="050ef-109">说明</span><span class="sxs-lookup"><span data-stu-id="050ef-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="050ef-110">name</span><span class="sxs-lookup"><span data-stu-id="050ef-110">name</span></span>|<span data-ttu-id="050ef-111">字符串</span><span class="sxs-lookup"><span data-stu-id="050ef-111">String</span></span>|<span data-ttu-id="050ef-112">证书控制名称</span><span class="sxs-lookup"><span data-stu-id="050ef-112">Certification control name</span></span> |
|<span data-ttu-id="050ef-113">url</span><span class="sxs-lookup"><span data-stu-id="050ef-113">url</span></span>|<span data-ttu-id="050ef-114">String</span><span class="sxs-lookup"><span data-stu-id="050ef-114">String</span></span>|<span data-ttu-id="050ef-115">Microsoft 服务信任门户的 URL</span><span class="sxs-lookup"><span data-stu-id="050ef-115">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="050ef-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="050ef-116">JSON representation</span></span>

<span data-ttu-id="050ef-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="050ef-117">The following is a JSON representation of the resource.</span></span>

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
