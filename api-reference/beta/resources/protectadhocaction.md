---
title: protectAdhocAction 资源类型
description: 通知应用程序应应用 ad hoc 保护。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f05273d19eec691d977a8810a5afa0c3fb22d28
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939079"
---
# <a name="protectadhocaction-resource-type"></a><span data-ttu-id="0da48-103">protectAdhocAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0da48-103">protectAdhocAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0da48-104">通知应用程序应应用 ad hoc 保护。</span><span class="sxs-lookup"><span data-stu-id="0da48-104">Informs the application that ad hoc protection should be applied.</span></span> <span data-ttu-id="0da48-105">**ProtectAdhocAction**通知应用程序该标签应应用临时保护。</span><span class="sxs-lookup"><span data-stu-id="0da48-105">The **protectAdhocAction** informs that applications that the label should apply ad hoc protection.</span></span> <span data-ttu-id="0da48-106">临时保护在运行时由用户或应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="0da48-106">Ad hoc protection is defined at runtime by the user or application.</span></span> <span data-ttu-id="0da48-107">使用应用程序必须使用 Microsoft 信息保护 SDK 在本地对文件或数据应用保护。</span><span class="sxs-lookup"><span data-stu-id="0da48-107">The consuming application must use the Microsoft Information Protection SDK to locally apply the protection to the file or data.</span></span>

## <a name="properties"></a><span data-ttu-id="0da48-108">属性</span><span class="sxs-lookup"><span data-stu-id="0da48-108">Properties</span></span>

<span data-ttu-id="0da48-109">无</span><span class="sxs-lookup"><span data-stu-id="0da48-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0da48-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0da48-110">JSON representation</span></span>

<span data-ttu-id="0da48-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0da48-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectAdhocAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectAdhocAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->