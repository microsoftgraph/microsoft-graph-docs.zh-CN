---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ac7c46dd21ffb9e9a31223822cf304e2b80c4f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215721"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="ff6fd-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff6fd-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="ff6fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff6fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff6fd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff6fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff6fd-107">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="ff6fd-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff6fd-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff6fd-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff6fd-109">Properties</span></span>
|<span data-ttu-id="ff6fd-110">属性</span><span class="sxs-lookup"><span data-stu-id="ff6fd-110">Property</span></span>|<span data-ttu-id="ff6fd-111">类型</span><span class="sxs-lookup"><span data-stu-id="ff6fd-111">Type</span></span>|<span data-ttu-id="ff6fd-112">说明</span><span class="sxs-lookup"><span data-stu-id="ff6fd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff6fd-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ff6fd-113">displayName</span></span>|<span data-ttu-id="ff6fd-114">String</span><span class="sxs-lookup"><span data-stu-id="ff6fd-114">String</span></span>|<span data-ttu-id="ff6fd-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-115">Display Name.</span></span> <span data-ttu-id="ff6fd-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff6fd-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff6fd-117">description</span><span class="sxs-lookup"><span data-stu-id="ff6fd-117">description</span></span>|<span data-ttu-id="ff6fd-118">String</span><span class="sxs-lookup"><span data-stu-id="ff6fd-118">String</span></span>|<span data-ttu-id="ff6fd-119">说明。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-119">Description.</span></span> <span data-ttu-id="ff6fd-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff6fd-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff6fd-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ff6fd-121">omaUri</span></span>|<span data-ttu-id="ff6fd-122">String</span><span class="sxs-lookup"><span data-stu-id="ff6fd-122">String</span></span>|<span data-ttu-id="ff6fd-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-123">OMA.</span></span> <span data-ttu-id="ff6fd-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff6fd-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff6fd-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ff6fd-125">isEncrypted</span></span>|<span data-ttu-id="ff6fd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6fd-126">Boolean</span></span>|<span data-ttu-id="ff6fd-127">指示是否对值字段进行加密。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="ff6fd-128">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff6fd-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff6fd-129">fileName</span><span class="sxs-lookup"><span data-stu-id="ff6fd-129">fileName</span></span>|<span data-ttu-id="ff6fd-130">String</span><span class="sxs-lookup"><span data-stu-id="ff6fd-130">String</span></span>|<span data-ttu-id="ff6fd-131">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-131">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="ff6fd-132">value</span><span class="sxs-lookup"><span data-stu-id="ff6fd-132">value</span></span>|<span data-ttu-id="ff6fd-133">Binary</span><span class="sxs-lookup"><span data-stu-id="ff6fd-133">Binary</span></span>|<span data-ttu-id="ff6fd-134">值。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-134">Value.</span></span> <span data-ttu-id="ff6fd-135">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="ff6fd-135">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff6fd-136">关系</span><span class="sxs-lookup"><span data-stu-id="ff6fd-136">Relationships</span></span>
<span data-ttu-id="ff6fd-137">无</span><span class="sxs-lookup"><span data-stu-id="ff6fd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff6fd-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff6fd-138">JSON Representation</span></span>
<span data-ttu-id="ff6fd-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff6fd-139">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "fileName": "String",
  "value": "binary"
}
```




