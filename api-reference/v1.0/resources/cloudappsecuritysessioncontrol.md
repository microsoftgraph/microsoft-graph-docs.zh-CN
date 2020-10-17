---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制实施云应用安全检查的会话控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 114e788e12ab8f633bc6350b08140f9d5e4fe8a3
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581265"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="89357-103">cloudAppSecuritySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="89357-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="89357-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89357-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89357-105">用于强制实施云应用安全检查的会话控制。</span><span class="sxs-lookup"><span data-stu-id="89357-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="89357-106">Inehrits 来自 [条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="89357-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="89357-107">属性</span><span class="sxs-lookup"><span data-stu-id="89357-107">Properties</span></span>

| <span data-ttu-id="89357-108">属性</span><span class="sxs-lookup"><span data-stu-id="89357-108">Property</span></span>     | <span data-ttu-id="89357-109">类型</span><span class="sxs-lookup"><span data-stu-id="89357-109">Type</span></span>        | <span data-ttu-id="89357-110">说明</span><span class="sxs-lookup"><span data-stu-id="89357-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89357-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="89357-111">isEnabled</span></span>     |<span data-ttu-id="89357-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="89357-112">Boolean</span></span>      | <span data-ttu-id="89357-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="89357-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="89357-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="89357-114">cloudAppSecurityType</span></span>|<span data-ttu-id="89357-115">String</span><span class="sxs-lookup"><span data-stu-id="89357-115">String</span></span>| <span data-ttu-id="89357-116">可能的值是：`mcasConfigured`、`monitorOnly`、`blockDownloads`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="89357-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="89357-117">有关详细信息，请参阅 [为特色应用程序部署条件访问应用控件](/cloud-app-security/proxy-deployment-aad)。</span><span class="sxs-lookup"><span data-stu-id="89357-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="89357-118">关系</span><span class="sxs-lookup"><span data-stu-id="89357-118">Relationships</span></span>

<span data-ttu-id="89357-119">无。</span><span class="sxs-lookup"><span data-stu-id="89357-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89357-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89357-120">JSON representation</span></span>

<span data-ttu-id="89357-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89357-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->