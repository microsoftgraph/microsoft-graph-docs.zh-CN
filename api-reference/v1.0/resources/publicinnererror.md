---
title: publicInnerError 资源类型
description: 表示错误的内部详细信息。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f089c120ac4ba1307f0b0ffa2f08f8578613eaa1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467298"
---
# <a name="publicinnererror-resource-type"></a><span data-ttu-id="daf16-103">publicInnerError 资源类型</span><span class="sxs-lookup"><span data-stu-id="daf16-103">publicInnerError resource type</span></span>

<span data-ttu-id="daf16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="daf16-105">表示 [publicError 的内部详细信息](../resources/publicerrordetail.md)。</span><span class="sxs-lookup"><span data-stu-id="daf16-105">Represents the inner details of a [publicError](../resources/publicerrordetail.md).</span></span> 
## <a name="properties"></a><span data-ttu-id="daf16-106">属性</span><span class="sxs-lookup"><span data-stu-id="daf16-106">Properties</span></span>
|<span data-ttu-id="daf16-107">属性</span><span class="sxs-lookup"><span data-stu-id="daf16-107">Property</span></span>|<span data-ttu-id="daf16-108">类型</span><span class="sxs-lookup"><span data-stu-id="daf16-108">Type</span></span>|<span data-ttu-id="daf16-109">说明</span><span class="sxs-lookup"><span data-stu-id="daf16-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf16-110">code</span><span class="sxs-lookup"><span data-stu-id="daf16-110">code</span></span>|<span data-ttu-id="daf16-111">String</span><span class="sxs-lookup"><span data-stu-id="daf16-111">String</span></span>|<span data-ttu-id="daf16-112">错误代码。</span><span class="sxs-lookup"><span data-stu-id="daf16-112">The error code.</span></span>|
|<span data-ttu-id="daf16-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="daf16-113">details</span></span>|<span data-ttu-id="daf16-114">[publicErrorDetail](../resources/publicerrordetail.md) 集合</span><span class="sxs-lookup"><span data-stu-id="daf16-114">[publicErrorDetail](../resources/publicerrordetail.md) collection</span></span>|<span data-ttu-id="daf16-115">错误详细信息的集合。</span><span class="sxs-lookup"><span data-stu-id="daf16-115">A collection of error details.</span></span>|
|<span data-ttu-id="daf16-116">message</span><span class="sxs-lookup"><span data-stu-id="daf16-116">message</span></span>|<span data-ttu-id="daf16-117">String</span><span class="sxs-lookup"><span data-stu-id="daf16-117">String</span></span>|<span data-ttu-id="daf16-118">错误消息。</span><span class="sxs-lookup"><span data-stu-id="daf16-118">The error message.</span></span>|
|<span data-ttu-id="daf16-119">target</span><span class="sxs-lookup"><span data-stu-id="daf16-119">target</span></span>|<span data-ttu-id="daf16-120">String</span><span class="sxs-lookup"><span data-stu-id="daf16-120">String</span></span>|<span data-ttu-id="daf16-121">错误的目标值。</span><span class="sxs-lookup"><span data-stu-id="daf16-121">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf16-122">关系</span><span class="sxs-lookup"><span data-stu-id="daf16-122">Relationships</span></span>
<span data-ttu-id="daf16-123">无。</span><span class="sxs-lookup"><span data-stu-id="daf16-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="daf16-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="daf16-124">JSON representation</span></span>
<span data-ttu-id="daf16-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daf16-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ]
}
```
