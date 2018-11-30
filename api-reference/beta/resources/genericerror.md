---
title: genericError 资源类型
description: 一个通用的错误。
ms.openlocfilehash: caf3fbb99ad521fd807138ab230f6a1b8ae7bb16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042164"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="a846e-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="a846e-103">genericError resource type</span></span>

> <span data-ttu-id="a846e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a846e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a846e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a846e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a846e-106">一个通用的错误。</span><span class="sxs-lookup"><span data-stu-id="a846e-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="a846e-107">属性</span><span class="sxs-lookup"><span data-stu-id="a846e-107">Properties</span></span>

| <span data-ttu-id="a846e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a846e-108">Property</span></span> | <span data-ttu-id="a846e-109">类型</span><span class="sxs-lookup"><span data-stu-id="a846e-109">Type</span></span> | <span data-ttu-id="a846e-110">说明</span><span class="sxs-lookup"><span data-stu-id="a846e-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a846e-111">message</span><span class="sxs-lookup"><span data-stu-id="a846e-111">message</span></span> | <span data-ttu-id="a846e-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a846e-112">String</span></span> | <span data-ttu-id="a846e-113">错误消息。</span><span class="sxs-lookup"><span data-stu-id="a846e-113">The error message.</span></span> |
| <span data-ttu-id="a846e-114">code</span><span class="sxs-lookup"><span data-stu-id="a846e-114">code</span></span> | <span data-ttu-id="a846e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="a846e-115">String</span></span> | <span data-ttu-id="a846e-116">错误代码。</span><span class="sxs-lookup"><span data-stu-id="a846e-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a846e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a846e-117">JSON representation</span></span>

<span data-ttu-id="a846e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a846e-118">Here is a JSON representation of the resource.</span></span>

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