---
title: publicErrorDetail 资源类型
description: 表示错误的详细信息。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac86f2aa50e1447702099f3c73f31979b6e6eb16
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467299"
---
# <a name="publicerrordetail-resource-type"></a><span data-ttu-id="530af-103">publicErrorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="530af-103">publicErrorDetail resource type</span></span>

<span data-ttu-id="530af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="530af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="530af-105">表示 [publicError 或](../resources/publicerror.md) [publicInnerError 的详细信息](../resources/publicinnererror.md)。</span><span class="sxs-lookup"><span data-stu-id="530af-105">Represents the details of [publicError](../resources/publicerror.md) or [publicInnerError](../resources/publicinnererror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="530af-106">属性</span><span class="sxs-lookup"><span data-stu-id="530af-106">Properties</span></span>
|<span data-ttu-id="530af-107">属性</span><span class="sxs-lookup"><span data-stu-id="530af-107">Property</span></span>|<span data-ttu-id="530af-108">类型</span><span class="sxs-lookup"><span data-stu-id="530af-108">Type</span></span>|<span data-ttu-id="530af-109">说明</span><span class="sxs-lookup"><span data-stu-id="530af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="530af-110">code</span><span class="sxs-lookup"><span data-stu-id="530af-110">code</span></span>|<span data-ttu-id="530af-111">String</span><span class="sxs-lookup"><span data-stu-id="530af-111">String</span></span>|<span data-ttu-id="530af-112">错误代码。</span><span class="sxs-lookup"><span data-stu-id="530af-112">The error code.</span></span>|
|<span data-ttu-id="530af-113">message</span><span class="sxs-lookup"><span data-stu-id="530af-113">message</span></span>|<span data-ttu-id="530af-114">String</span><span class="sxs-lookup"><span data-stu-id="530af-114">String</span></span>|<span data-ttu-id="530af-115">错误消息。</span><span class="sxs-lookup"><span data-stu-id="530af-115">The error message.</span></span>|
|<span data-ttu-id="530af-116">target</span><span class="sxs-lookup"><span data-stu-id="530af-116">target</span></span>|<span data-ttu-id="530af-117">String</span><span class="sxs-lookup"><span data-stu-id="530af-117">String</span></span>|<span data-ttu-id="530af-118">错误的目标值。</span><span class="sxs-lookup"><span data-stu-id="530af-118">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="530af-119">关系</span><span class="sxs-lookup"><span data-stu-id="530af-119">Relationships</span></span>
<span data-ttu-id="530af-120">无。</span><span class="sxs-lookup"><span data-stu-id="530af-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="530af-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="530af-121">JSON representation</span></span>
<span data-ttu-id="530af-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="530af-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```
