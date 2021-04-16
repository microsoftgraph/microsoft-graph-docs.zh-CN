---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e05111209d50fec1aee52a5e9ee87baae3ca47a1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867446"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="8d16a-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d16a-103">omaSetting resource type</span></span>

<span data-ttu-id="8d16a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d16a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d16a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d16a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d16a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d16a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d16a-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="8d16a-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8d16a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d16a-108">Properties</span></span>
|<span data-ttu-id="8d16a-109">属性</span><span class="sxs-lookup"><span data-stu-id="8d16a-109">Property</span></span>|<span data-ttu-id="8d16a-110">类型</span><span class="sxs-lookup"><span data-stu-id="8d16a-110">Type</span></span>|<span data-ttu-id="8d16a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8d16a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d16a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8d16a-112">displayName</span></span>|<span data-ttu-id="8d16a-113">String</span><span class="sxs-lookup"><span data-stu-id="8d16a-113">String</span></span>|<span data-ttu-id="8d16a-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="8d16a-114">Display Name.</span></span>|
|<span data-ttu-id="8d16a-115">说明</span><span class="sxs-lookup"><span data-stu-id="8d16a-115">description</span></span>|<span data-ttu-id="8d16a-116">String</span><span class="sxs-lookup"><span data-stu-id="8d16a-116">String</span></span>|<span data-ttu-id="8d16a-117">说明。</span><span class="sxs-lookup"><span data-stu-id="8d16a-117">Description.</span></span>|
|<span data-ttu-id="8d16a-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="8d16a-118">omaUri</span></span>|<span data-ttu-id="8d16a-119">String</span><span class="sxs-lookup"><span data-stu-id="8d16a-119">String</span></span>|<span data-ttu-id="8d16a-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="8d16a-120">OMA.</span></span>|
|<span data-ttu-id="8d16a-121">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="8d16a-121">secretReferenceValueId</span></span>|<span data-ttu-id="8d16a-122">String</span><span class="sxs-lookup"><span data-stu-id="8d16a-122">String</span></span>|<span data-ttu-id="8d16a-123">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="8d16a-123">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="8d16a-124">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8d16a-124">This property is read-only.</span></span>|
|<span data-ttu-id="8d16a-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="8d16a-125">isEncrypted</span></span>|<span data-ttu-id="8d16a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d16a-126">Boolean</span></span>|<span data-ttu-id="8d16a-127">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="8d16a-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="8d16a-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8d16a-128">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d16a-129">关系</span><span class="sxs-lookup"><span data-stu-id="8d16a-129">Relationships</span></span>
<span data-ttu-id="8d16a-130">无</span><span class="sxs-lookup"><span data-stu-id="8d16a-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d16a-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d16a-131">JSON Representation</span></span>
<span data-ttu-id="8d16a-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d16a-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true
}
```




