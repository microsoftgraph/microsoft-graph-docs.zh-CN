---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制执行的关键限制。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a40a185f688038d3c849113ae8e9b53c4f0652f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133796"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="840d6-103">fido2KeyRestrictions 资源类型</span><span class="sxs-lookup"><span data-stu-id="840d6-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="840d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="840d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="840d6-105">表示作为 FIDO2 安全密钥身份验证方法策略的一部分 [强制执行的关键限制](../resources/fido2authenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="840d6-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="840d6-106">属性</span><span class="sxs-lookup"><span data-stu-id="840d6-106">Properties</span></span>
|<span data-ttu-id="840d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="840d6-107">Property</span></span>|<span data-ttu-id="840d6-108">类型</span><span class="sxs-lookup"><span data-stu-id="840d6-108">Type</span></span>|<span data-ttu-id="840d6-109">说明</span><span class="sxs-lookup"><span data-stu-id="840d6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="840d6-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="840d6-110">aaGuids</span></span>|<span data-ttu-id="840d6-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="840d6-111">String collection</span></span>|<span data-ttu-id="840d6-112">Authenticator 证明 GUID 的集合。</span><span class="sxs-lookup"><span data-stu-id="840d6-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="840d6-113">AADGUID 定义密钥类型和制造商。</span><span class="sxs-lookup"><span data-stu-id="840d6-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="840d6-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="840d6-114">enforcementType</span></span>|<span data-ttu-id="840d6-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="840d6-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="840d6-116">强制类型。</span><span class="sxs-lookup"><span data-stu-id="840d6-116">Enforcement type.</span></span> <span data-ttu-id="840d6-117">可取值为：`allow`、`block`。</span><span class="sxs-lookup"><span data-stu-id="840d6-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="840d6-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="840d6-118">isEnforced</span></span>|<span data-ttu-id="840d6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="840d6-119">Boolean</span></span>|<span data-ttu-id="840d6-120">确定是否启用已配置的密钥强制。</span><span class="sxs-lookup"><span data-stu-id="840d6-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="840d6-121">关系</span><span class="sxs-lookup"><span data-stu-id="840d6-121">Relationships</span></span>
<span data-ttu-id="840d6-122">无。</span><span class="sxs-lookup"><span data-stu-id="840d6-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="840d6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="840d6-123">JSON representation</span></span>
<span data-ttu-id="840d6-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="840d6-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
