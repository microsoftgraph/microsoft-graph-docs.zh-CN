---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制执行云应用安全检查的会话控制。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b1eee93b3f80b6d7d916f38d783ca94cef8e81a1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133054"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="2c24e-103">cloudAppSecuritySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c24e-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="2c24e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c24e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c24e-105">用于强制执行云应用安全检查的会话控制。</span><span class="sxs-lookup"><span data-stu-id="2c24e-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="2c24e-106">条件访问会话 [控件中的指令](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="2c24e-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c24e-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c24e-107">Properties</span></span>

| <span data-ttu-id="2c24e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c24e-108">Property</span></span>     | <span data-ttu-id="2c24e-109">类型</span><span class="sxs-lookup"><span data-stu-id="2c24e-109">Type</span></span>        | <span data-ttu-id="2c24e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2c24e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c24e-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2c24e-111">isEnabled</span></span>     |<span data-ttu-id="2c24e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c24e-112">Boolean</span></span>      | <span data-ttu-id="2c24e-113">指定是否启用会话控件。</span><span class="sxs-lookup"><span data-stu-id="2c24e-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="2c24e-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="2c24e-114">cloudAppSecurityType</span></span>|<span data-ttu-id="2c24e-115">String</span><span class="sxs-lookup"><span data-stu-id="2c24e-115">String</span></span>| <span data-ttu-id="2c24e-116">可能的值是：`mcasConfigured`、`monitorOnly`、`blockDownloads`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2c24e-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="2c24e-117">有关详细信息，请参阅为特别推荐 [的应用部署条件访问应用控件](/cloud-app-security/proxy-deployment-aad)。</span><span class="sxs-lookup"><span data-stu-id="2c24e-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c24e-118">关系</span><span class="sxs-lookup"><span data-stu-id="2c24e-118">Relationships</span></span>

<span data-ttu-id="2c24e-119">无。</span><span class="sxs-lookup"><span data-stu-id="2c24e-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c24e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c24e-120">JSON representation</span></span>

<span data-ttu-id="2c24e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c24e-121">The following is a JSON representation of the resource.</span></span>

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
