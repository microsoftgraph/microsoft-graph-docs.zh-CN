---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制实施云应用安全检查的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 105a60905bd69317d152d9609e0a95fb78610a35
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638594"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="318e3-103">cloudAppSecuritySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="318e3-103">cloudAppSecuritySessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="318e3-104">用于强制实施云应用安全检查的会话控制。</span><span class="sxs-lookup"><span data-stu-id="318e3-104">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="318e3-105">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="318e3-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="318e3-106">属性</span><span class="sxs-lookup"><span data-stu-id="318e3-106">Properties</span></span>

| <span data-ttu-id="318e3-107">属性</span><span class="sxs-lookup"><span data-stu-id="318e3-107">Property</span></span>     | <span data-ttu-id="318e3-108">类型</span><span class="sxs-lookup"><span data-stu-id="318e3-108">Type</span></span>        | <span data-ttu-id="318e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="318e3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="318e3-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="318e3-110">isEnabled</span></span>     |<span data-ttu-id="318e3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="318e3-111">Boolean</span></span>      | <span data-ttu-id="318e3-112">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="318e3-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="318e3-113">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="318e3-113">cloudAppSecurityType</span></span>|<span data-ttu-id="318e3-114">String</span><span class="sxs-lookup"><span data-stu-id="318e3-114">String</span></span> | <span data-ttu-id="318e3-115">可取值为：`mcasConfigured`、`monitorOnly`、`blockDownloads`。</span><span class="sxs-lookup"><span data-stu-id="318e3-115">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="318e3-116">请在此处了解有关这些值的详细信息：https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="318e3-116">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="318e3-117">关系</span><span class="sxs-lookup"><span data-stu-id="318e3-117">Relationships</span></span>

<span data-ttu-id="318e3-118">无。</span><span class="sxs-lookup"><span data-stu-id="318e3-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="318e3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="318e3-119">JSON representation</span></span>

<span data-ttu-id="318e3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="318e3-120">The following is a JSON representation of the resource.</span></span>

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