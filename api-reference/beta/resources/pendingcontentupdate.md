---
title: pendingContentUpdate
description: PendingContentUpdate 资源指示可能影响 driveItem 的二进制内容的操作处于 "正在等待" 已完成。
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7862d8da186448d08d6dfd5691ae83e29bd57a5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521974"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="26807-103">pendingContentUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="26807-103">pendingContentUpdate resource type</span></span>

<span data-ttu-id="26807-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="26807-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26807-105">指示可能会影响**driveItem**的二进制内容的操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="26807-105">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="26807-106">属性</span><span class="sxs-lookup"><span data-stu-id="26807-106">Properties</span></span>

| <span data-ttu-id="26807-107">属性</span><span class="sxs-lookup"><span data-stu-id="26807-107">Property</span></span>     | <span data-ttu-id="26807-108">类型</span><span class="sxs-lookup"><span data-stu-id="26807-108">Type</span></span>         | <span data-ttu-id="26807-109">说明</span><span class="sxs-lookup"><span data-stu-id="26807-109">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="26807-110">queuedDateTime</span><span class="sxs-lookup"><span data-stu-id="26807-110">queuedDateTime</span></span>|<span data-ttu-id="26807-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26807-111">DateTimeOffset</span></span>|<span data-ttu-id="26807-112">在 UTC 时间内排队待执行的二进制操作的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="26807-112">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="26807-113">只读。</span><span class="sxs-lookup"><span data-stu-id="26807-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26807-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26807-114">JSON representation</span></span>

<span data-ttu-id="26807-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26807-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
