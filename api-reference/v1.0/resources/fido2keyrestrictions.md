---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制执行的关键限制。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fd319b64d124fc2c80c7f851a2e062d3568c2d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964683"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="b3cc1-103">fido2KeyRestrictions 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3cc1-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="b3cc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3cc1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3cc1-105">表示作为 [FIDO2](../resources/fido2authenticationmethodconfiguration.md)安全密钥身份验证方法策略的一部分强制执行的关键限制。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b3cc1-106">属性</span><span class="sxs-lookup"><span data-stu-id="b3cc1-106">Properties</span></span>
|<span data-ttu-id="b3cc1-107">属性</span><span class="sxs-lookup"><span data-stu-id="b3cc1-107">Property</span></span>|<span data-ttu-id="b3cc1-108">类型</span><span class="sxs-lookup"><span data-stu-id="b3cc1-108">Type</span></span>|<span data-ttu-id="b3cc1-109">说明</span><span class="sxs-lookup"><span data-stu-id="b3cc1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3cc1-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="b3cc1-110">aaGuids</span></span>|<span data-ttu-id="b3cc1-111">String collection</span><span class="sxs-lookup"><span data-stu-id="b3cc1-111">String collection</span></span>|<span data-ttu-id="b3cc1-112">Authenticator 证明 GUID 的集合。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="b3cc1-113">AADGUIDs 定义密钥类型和制造商。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="b3cc1-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="b3cc1-114">enforcementType</span></span>|<span data-ttu-id="b3cc1-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="b3cc1-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="b3cc1-116">强制类型。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-116">Enforcement type.</span></span> <span data-ttu-id="b3cc1-117">可取值为：`allow`、`block`。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="b3cc1-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="b3cc1-118">isEnforced</span></span>|<span data-ttu-id="b3cc1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3cc1-119">Boolean</span></span>|<span data-ttu-id="b3cc1-120">确定是否启用配置的密钥强制。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3cc1-121">关系</span><span class="sxs-lookup"><span data-stu-id="b3cc1-121">Relationships</span></span>
<span data-ttu-id="b3cc1-122">无。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3cc1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3cc1-123">JSON representation</span></span>
<span data-ttu-id="b3cc1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3cc1-124">The following is a JSON representation of the resource.</span></span>
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
