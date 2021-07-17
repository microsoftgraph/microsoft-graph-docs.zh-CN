---
title: publicError 资源类型
description: 表示一般错误及其详细信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: e9f5decf8edc2ebf3e11d00eb89e68236a6a73d4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467301"
---
# <a name="publicerror-resource-type"></a><span data-ttu-id="ad7b1-103">publicError 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad7b1-103">publicError resource type</span></span>

<span data-ttu-id="ad7b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad7b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad7b1-105">表示一般错误及其详细信息。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-105">Represents a generic error and its details.</span></span>

## <a name="properties"></a><span data-ttu-id="ad7b1-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad7b1-106">Properties</span></span>
|<span data-ttu-id="ad7b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad7b1-107">Property</span></span>|<span data-ttu-id="ad7b1-108">类型</span><span class="sxs-lookup"><span data-stu-id="ad7b1-108">Type</span></span>|<span data-ttu-id="ad7b1-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad7b1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad7b1-110">code</span><span class="sxs-lookup"><span data-stu-id="ad7b1-110">code</span></span>|<span data-ttu-id="ad7b1-111">string</span><span class="sxs-lookup"><span data-stu-id="ad7b1-111">string</span></span>| <span data-ttu-id="ad7b1-112">表示错误代码。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-112">Represents the error code.</span></span>
|<span data-ttu-id="ad7b1-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="ad7b1-113">details</span></span>|<span data-ttu-id="ad7b1-114">[publicErrorDetail](publicerrordetail.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ad7b1-114">[publicErrorDetail](publicerrordetail.md) collection</span></span>|<span data-ttu-id="ad7b1-115">错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-115">Details of the error.</span></span>|
|<span data-ttu-id="ad7b1-116">innerError</span><span class="sxs-lookup"><span data-stu-id="ad7b1-116">innerError</span></span>|[<span data-ttu-id="ad7b1-117">publicInnerError</span><span class="sxs-lookup"><span data-stu-id="ad7b1-117">publicInnerError</span></span>](publicinnererror.md)|<span data-ttu-id="ad7b1-118">内部错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-118">Details of the inner error.</span></span>|
|<span data-ttu-id="ad7b1-119">message</span><span class="sxs-lookup"><span data-stu-id="ad7b1-119">message</span></span>|<span data-ttu-id="ad7b1-120">字符串</span><span class="sxs-lookup"><span data-stu-id="ad7b1-120">string</span></span>| <span data-ttu-id="ad7b1-121">针对开发人员的非本地化邮件。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-121">A non-localized message for the developer.</span></span>
|<span data-ttu-id="ad7b1-122">target</span><span class="sxs-lookup"><span data-stu-id="ad7b1-122">target</span></span>|<span data-ttu-id="ad7b1-123">String</span><span class="sxs-lookup"><span data-stu-id="ad7b1-123">String</span></span>|<span data-ttu-id="ad7b1-124">错误的目标值。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-124">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad7b1-125">关系</span><span class="sxs-lookup"><span data-stu-id="ad7b1-125">Relationships</span></span>
<span data-ttu-id="ad7b1-126">无。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad7b1-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad7b1-127">JSON representation</span></span>
<span data-ttu-id="ad7b1-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad7b1-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```
