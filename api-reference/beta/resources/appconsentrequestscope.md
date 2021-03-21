---
title: appConsentRequestScope 资源类型
description: 请求访问的动态权限范围的详细信息。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b960820e0d7cf20a37850256bb96ba3abf034038
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965114"
---
# <a name="appconsentrequestscope-resource-type"></a><span data-ttu-id="61c2e-103">appConsentRequestScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="61c2e-103">appConsentRequestScope resource type</span></span>

<span data-ttu-id="61c2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61c2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61c2e-105">**appConsentRequestScope** 详细介绍了请求访问的动态权限范围。</span><span class="sxs-lookup"><span data-stu-id="61c2e-105">The **appConsentRequestScope** details the dynamic permission scopes for which access is being requested.</span></span>

## <a name="properties"></a><span data-ttu-id="61c2e-106">属性</span><span class="sxs-lookup"><span data-stu-id="61c2e-106">Properties</span></span>
|<span data-ttu-id="61c2e-107">属性</span><span class="sxs-lookup"><span data-stu-id="61c2e-107">Property</span></span>|<span data-ttu-id="61c2e-108">类型</span><span class="sxs-lookup"><span data-stu-id="61c2e-108">Type</span></span>|<span data-ttu-id="61c2e-109">说明</span><span class="sxs-lookup"><span data-stu-id="61c2e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c2e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="61c2e-110">displayName</span></span>|<span data-ttu-id="61c2e-111">String</span><span class="sxs-lookup"><span data-stu-id="61c2e-111">String</span></span>|<span data-ttu-id="61c2e-112">范围的名称。</span><span class="sxs-lookup"><span data-stu-id="61c2e-112">The name of the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61c2e-113">关系</span><span class="sxs-lookup"><span data-stu-id="61c2e-113">Relationships</span></span>
<span data-ttu-id="61c2e-114">无。</span><span class="sxs-lookup"><span data-stu-id="61c2e-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61c2e-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61c2e-115">JSON representation</span></span>
<span data-ttu-id="61c2e-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61c2e-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConsentRequestScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequestScope",
  "displayName": "String"
}
```

