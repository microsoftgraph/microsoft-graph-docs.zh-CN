---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b899a076a291061649adab4724a9108d982886f5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867369"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="eedfd-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="eedfd-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="eedfd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eedfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eedfd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eedfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eedfd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eedfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eedfd-107">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="eedfd-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="eedfd-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eedfd-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eedfd-109">属性</span><span class="sxs-lookup"><span data-stu-id="eedfd-109">Properties</span></span>
|<span data-ttu-id="eedfd-110">属性</span><span class="sxs-lookup"><span data-stu-id="eedfd-110">Property</span></span>|<span data-ttu-id="eedfd-111">类型</span><span class="sxs-lookup"><span data-stu-id="eedfd-111">Type</span></span>|<span data-ttu-id="eedfd-112">说明</span><span class="sxs-lookup"><span data-stu-id="eedfd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eedfd-113">displayName</span><span class="sxs-lookup"><span data-stu-id="eedfd-113">displayName</span></span>|<span data-ttu-id="eedfd-114">String</span><span class="sxs-lookup"><span data-stu-id="eedfd-114">String</span></span>|<span data-ttu-id="eedfd-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="eedfd-115">Display Name.</span></span> <span data-ttu-id="eedfd-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eedfd-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eedfd-117">说明</span><span class="sxs-lookup"><span data-stu-id="eedfd-117">description</span></span>|<span data-ttu-id="eedfd-118">String</span><span class="sxs-lookup"><span data-stu-id="eedfd-118">String</span></span>|<span data-ttu-id="eedfd-119">说明。</span><span class="sxs-lookup"><span data-stu-id="eedfd-119">Description.</span></span> <span data-ttu-id="eedfd-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eedfd-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eedfd-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="eedfd-121">omaUri</span></span>|<span data-ttu-id="eedfd-122">String</span><span class="sxs-lookup"><span data-stu-id="eedfd-122">String</span></span>|<span data-ttu-id="eedfd-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="eedfd-123">OMA.</span></span> <span data-ttu-id="eedfd-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eedfd-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eedfd-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="eedfd-125">secretReferenceValueId</span></span>|<span data-ttu-id="eedfd-126">String</span><span class="sxs-lookup"><span data-stu-id="eedfd-126">String</span></span>|<span data-ttu-id="eedfd-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="eedfd-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="eedfd-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="eedfd-128">This property is read-only.</span></span> <span data-ttu-id="eedfd-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eedfd-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eedfd-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="eedfd-130">isEncrypted</span></span>|<span data-ttu-id="eedfd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="eedfd-131">Boolean</span></span>|<span data-ttu-id="eedfd-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="eedfd-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="eedfd-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="eedfd-133">This property is read-only.</span></span> <span data-ttu-id="eedfd-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eedfd-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eedfd-135">fileName</span><span class="sxs-lookup"><span data-stu-id="eedfd-135">fileName</span></span>|<span data-ttu-id="eedfd-136">String</span><span class="sxs-lookup"><span data-stu-id="eedfd-136">String</span></span>|<span data-ttu-id="eedfd-137">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="eedfd-137">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="eedfd-138">value</span><span class="sxs-lookup"><span data-stu-id="eedfd-138">value</span></span>|<span data-ttu-id="eedfd-139">Binary</span><span class="sxs-lookup"><span data-stu-id="eedfd-139">Binary</span></span>|<span data-ttu-id="eedfd-140">值。</span><span class="sxs-lookup"><span data-stu-id="eedfd-140">Value.</span></span> <span data-ttu-id="eedfd-141">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="eedfd-141">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="eedfd-142">关系</span><span class="sxs-lookup"><span data-stu-id="eedfd-142">Relationships</span></span>
<span data-ttu-id="eedfd-143">无</span><span class="sxs-lookup"><span data-stu-id="eedfd-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eedfd-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eedfd-144">JSON Representation</span></span>
<span data-ttu-id="eedfd-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eedfd-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "binary"
}
```




