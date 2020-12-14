---
title: publicErrorDetail 资源类型
description: 表示错误的详细信息。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8620d19d1cd540f7ed523a392e71c304cbbf1774
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659399"
---
# <a name="publicerrordetail-resource-type"></a><span data-ttu-id="79b24-103">publicErrorDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="79b24-103">publicErrorDetail resource type</span></span>

<span data-ttu-id="79b24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79b24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79b24-105">表示 [publicError 或](../resources/publicerror.md) [publicInnerError 的详细信息](../resources/publicinnererror.md)。</span><span class="sxs-lookup"><span data-stu-id="79b24-105">Represents the details of [publicError](../resources/publicerror.md) or [publicInnerError](../resources/publicinnererror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="79b24-106">属性</span><span class="sxs-lookup"><span data-stu-id="79b24-106">Properties</span></span>
|<span data-ttu-id="79b24-107">属性</span><span class="sxs-lookup"><span data-stu-id="79b24-107">Property</span></span>|<span data-ttu-id="79b24-108">类型</span><span class="sxs-lookup"><span data-stu-id="79b24-108">Type</span></span>|<span data-ttu-id="79b24-109">说明</span><span class="sxs-lookup"><span data-stu-id="79b24-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79b24-110">code</span><span class="sxs-lookup"><span data-stu-id="79b24-110">code</span></span>|<span data-ttu-id="79b24-111">String</span><span class="sxs-lookup"><span data-stu-id="79b24-111">String</span></span>|<span data-ttu-id="79b24-112">错误代码。</span><span class="sxs-lookup"><span data-stu-id="79b24-112">The error code.</span></span>|
|<span data-ttu-id="79b24-113">message</span><span class="sxs-lookup"><span data-stu-id="79b24-113">message</span></span>|<span data-ttu-id="79b24-114">String</span><span class="sxs-lookup"><span data-stu-id="79b24-114">String</span></span>|<span data-ttu-id="79b24-115">错误消息。</span><span class="sxs-lookup"><span data-stu-id="79b24-115">The error message.</span></span>|
|<span data-ttu-id="79b24-116">target</span><span class="sxs-lookup"><span data-stu-id="79b24-116">target</span></span>|<span data-ttu-id="79b24-117">String</span><span class="sxs-lookup"><span data-stu-id="79b24-117">String</span></span>|<span data-ttu-id="79b24-118">错误的目标值。</span><span class="sxs-lookup"><span data-stu-id="79b24-118">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79b24-119">关系</span><span class="sxs-lookup"><span data-stu-id="79b24-119">Relationships</span></span>
<span data-ttu-id="79b24-120">无。</span><span class="sxs-lookup"><span data-stu-id="79b24-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79b24-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79b24-121">JSON representation</span></span>
<span data-ttu-id="79b24-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79b24-122">The following is a JSON representation of the resource.</span></span>
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

