---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 5a583c91c6f5b89ba594e0345c9c8cb256993f71
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812279"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="630ae-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="630ae-103">genericError resource type</span></span>

<span data-ttu-id="630ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="630ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="630ae-105">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="630ae-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="630ae-106">属性</span><span class="sxs-lookup"><span data-stu-id="630ae-106">Properties</span></span>

| <span data-ttu-id="630ae-107">属性</span><span class="sxs-lookup"><span data-stu-id="630ae-107">Property</span></span> | <span data-ttu-id="630ae-108">类型</span><span class="sxs-lookup"><span data-stu-id="630ae-108">Type</span></span> | <span data-ttu-id="630ae-109">描述</span><span class="sxs-lookup"><span data-stu-id="630ae-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="630ae-110">message</span><span class="sxs-lookup"><span data-stu-id="630ae-110">message</span></span> | <span data-ttu-id="630ae-111">String</span><span class="sxs-lookup"><span data-stu-id="630ae-111">String</span></span> | <span data-ttu-id="630ae-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="630ae-112">The error message.</span></span> |
| <span data-ttu-id="630ae-113">code</span><span class="sxs-lookup"><span data-stu-id="630ae-113">code</span></span> | <span data-ttu-id="630ae-114">String</span><span class="sxs-lookup"><span data-stu-id="630ae-114">String</span></span> | <span data-ttu-id="630ae-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="630ae-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="630ae-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="630ae-116">JSON representation</span></span>

<span data-ttu-id="630ae-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="630ae-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
