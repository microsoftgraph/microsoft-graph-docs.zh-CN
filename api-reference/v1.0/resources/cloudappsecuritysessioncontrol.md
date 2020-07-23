---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制实施云应用安全检查的会话控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6271ae47f94abb0c449dc6bd7a0930468d08d2b5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384485"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="52325-103">cloudAppSecuritySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="52325-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="52325-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52325-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52325-105">用于强制实施云应用安全检查的会话控制。</span><span class="sxs-lookup"><span data-stu-id="52325-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="52325-106">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="52325-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="52325-107">属性</span><span class="sxs-lookup"><span data-stu-id="52325-107">Properties</span></span>

| <span data-ttu-id="52325-108">属性</span><span class="sxs-lookup"><span data-stu-id="52325-108">Property</span></span>     | <span data-ttu-id="52325-109">类型</span><span class="sxs-lookup"><span data-stu-id="52325-109">Type</span></span>        | <span data-ttu-id="52325-110">说明</span><span class="sxs-lookup"><span data-stu-id="52325-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52325-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="52325-111">isEnabled</span></span>     |<span data-ttu-id="52325-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="52325-112">Boolean</span></span>      | <span data-ttu-id="52325-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="52325-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="52325-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="52325-114">cloudAppSecurityType</span></span>|<span data-ttu-id="52325-115">String</span><span class="sxs-lookup"><span data-stu-id="52325-115">String</span></span>| <span data-ttu-id="52325-116">可能的值是：`mcasConfigured`、`monitorOnly`、`blockDownloads`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="52325-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="52325-117">有关详细信息，请参阅[为特色应用程序部署条件访问应用控件](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad)。</span><span class="sxs-lookup"><span data-stu-id="52325-117">For more information, see [Deploy Conditional Access App Control for featured apps](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="52325-118">关系</span><span class="sxs-lookup"><span data-stu-id="52325-118">Relationships</span></span>

<span data-ttu-id="52325-119">无。</span><span class="sxs-lookup"><span data-stu-id="52325-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52325-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52325-120">JSON representation</span></span>

<span data-ttu-id="52325-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52325-121">The following is a JSON representation of the resource.</span></span>

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
