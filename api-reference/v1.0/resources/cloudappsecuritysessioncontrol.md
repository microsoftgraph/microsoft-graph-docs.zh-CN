---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制执行云应用安全检查的会话控制。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c52322928b5ef2e2538031ae8c251bc9c1a4caac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962509"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="73c9d-103">cloudAppSecuritySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="73c9d-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="73c9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73c9d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73c9d-105">用于强制执行云应用安全检查的会话控制。</span><span class="sxs-lookup"><span data-stu-id="73c9d-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="73c9d-106">条件访问会话 [控件中的指令](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="73c9d-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="73c9d-107">属性</span><span class="sxs-lookup"><span data-stu-id="73c9d-107">Properties</span></span>

| <span data-ttu-id="73c9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="73c9d-108">Property</span></span>     | <span data-ttu-id="73c9d-109">类型</span><span class="sxs-lookup"><span data-stu-id="73c9d-109">Type</span></span>        | <span data-ttu-id="73c9d-110">说明</span><span class="sxs-lookup"><span data-stu-id="73c9d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73c9d-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="73c9d-111">isEnabled</span></span>     |<span data-ttu-id="73c9d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c9d-112">Boolean</span></span>      | <span data-ttu-id="73c9d-113">指定是否启用会话控件。</span><span class="sxs-lookup"><span data-stu-id="73c9d-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="73c9d-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="73c9d-114">cloudAppSecurityType</span></span>|<span data-ttu-id="73c9d-115">cloudAppSecuritySessionControlType</span><span class="sxs-lookup"><span data-stu-id="73c9d-115">cloudAppSecuritySessionControlType</span></span>| <span data-ttu-id="73c9d-116">可取值为：`mcasConfigured`、`monitorOnly`、`blockDownloads`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="73c9d-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="73c9d-117">有关详细信息，请参阅为特色 [应用部署条件访问应用控制](/cloud-app-security/proxy-deployment-aad)。</span><span class="sxs-lookup"><span data-stu-id="73c9d-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="73c9d-118">关系</span><span class="sxs-lookup"><span data-stu-id="73c9d-118">Relationships</span></span>

<span data-ttu-id="73c9d-119">无。</span><span class="sxs-lookup"><span data-stu-id="73c9d-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73c9d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73c9d-120">JSON representation</span></span>

<span data-ttu-id="73c9d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73c9d-121">The following is a JSON representation of the resource.</span></span>

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
