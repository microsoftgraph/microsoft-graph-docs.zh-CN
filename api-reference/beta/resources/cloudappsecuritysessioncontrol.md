---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制实施云应用安全检查的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35f031498fb3a2f4f9c3a48d0102d57081b7c4d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507647"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="2661f-103">cloudAppSecuritySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="2661f-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="2661f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2661f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2661f-105">用于强制实施云应用安全检查的会话控制。</span><span class="sxs-lookup"><span data-stu-id="2661f-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="2661f-106">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="2661f-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2661f-107">属性</span><span class="sxs-lookup"><span data-stu-id="2661f-107">Properties</span></span>

| <span data-ttu-id="2661f-108">属性</span><span class="sxs-lookup"><span data-stu-id="2661f-108">Property</span></span>     | <span data-ttu-id="2661f-109">类型</span><span class="sxs-lookup"><span data-stu-id="2661f-109">Type</span></span>        | <span data-ttu-id="2661f-110">说明</span><span class="sxs-lookup"><span data-stu-id="2661f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2661f-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2661f-111">isEnabled</span></span>     |<span data-ttu-id="2661f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2661f-112">Boolean</span></span>      | <span data-ttu-id="2661f-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="2661f-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="2661f-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="2661f-114">cloudAppSecurityType</span></span>|<span data-ttu-id="2661f-115">String</span><span class="sxs-lookup"><span data-stu-id="2661f-115">String</span></span> | <span data-ttu-id="2661f-116">可取值为：`mcasConfigured`、`monitorOnly`、`blockDownloads`。</span><span class="sxs-lookup"><span data-stu-id="2661f-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="2661f-117">请在此处了解有关这些值的详细信息：https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="2661f-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="2661f-118">关系</span><span class="sxs-lookup"><span data-stu-id="2661f-118">Relationships</span></span>

<span data-ttu-id="2661f-119">无。</span><span class="sxs-lookup"><span data-stu-id="2661f-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2661f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2661f-120">JSON representation</span></span>

<span data-ttu-id="2661f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2661f-121">The following is a JSON representation of the resource.</span></span>

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