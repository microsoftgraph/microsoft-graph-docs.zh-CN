---
title: protectAdhocAction 资源类型
description: 通知应用程序应应用 ad hoc 保护。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd98c3cda25c435c27d912a4c896e7825be94340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521374"
---
# <a name="protectadhocaction-resource-type"></a><span data-ttu-id="b8056-103">protectAdhocAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8056-103">protectAdhocAction resource type</span></span>

<span data-ttu-id="b8056-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b8056-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8056-105">通知应用程序应应用 ad hoc 保护。</span><span class="sxs-lookup"><span data-stu-id="b8056-105">Informs the application that ad hoc protection should be applied.</span></span> <span data-ttu-id="b8056-106">**ProtectAdhocAction**通知应用程序该标签应应用临时保护。</span><span class="sxs-lookup"><span data-stu-id="b8056-106">The **protectAdhocAction** informs that applications that the label should apply ad hoc protection.</span></span> <span data-ttu-id="b8056-107">临时保护在运行时由用户或应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="b8056-107">Ad hoc protection is defined at runtime by the user or application.</span></span> <span data-ttu-id="b8056-108">使用应用程序必须使用 Microsoft 信息保护 SDK 在本地对文件或数据应用保护。</span><span class="sxs-lookup"><span data-stu-id="b8056-108">The consuming application must use the Microsoft Information Protection SDK to locally apply the protection to the file or data.</span></span>

## <a name="properties"></a><span data-ttu-id="b8056-109">属性</span><span class="sxs-lookup"><span data-stu-id="b8056-109">Properties</span></span>

<span data-ttu-id="b8056-110">无</span><span class="sxs-lookup"><span data-stu-id="b8056-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8056-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8056-111">JSON representation</span></span>

<span data-ttu-id="b8056-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8056-112">The following is a JSON representation of the resource.</span></span>

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