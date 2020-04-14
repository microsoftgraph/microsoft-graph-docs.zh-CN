---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ef4b46f375757419f63f11e0178ed4ab9ea5e11
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437071"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="9dd9e-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="9dd9e-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="9dd9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dd9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9dd9e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dd9e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd9e-107">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="9dd9e-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9dd9e-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9dd9e-109">属性</span><span class="sxs-lookup"><span data-stu-id="9dd9e-109">Properties</span></span>
|<span data-ttu-id="9dd9e-110">属性</span><span class="sxs-lookup"><span data-stu-id="9dd9e-110">Property</span></span>|<span data-ttu-id="9dd9e-111">类型</span><span class="sxs-lookup"><span data-stu-id="9dd9e-111">Type</span></span>|<span data-ttu-id="9dd9e-112">说明</span><span class="sxs-lookup"><span data-stu-id="9dd9e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd9e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd9e-113">displayName</span></span>|<span data-ttu-id="9dd9e-114">字符串</span><span class="sxs-lookup"><span data-stu-id="9dd9e-114">String</span></span>|<span data-ttu-id="9dd9e-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-115">Display Name.</span></span> <span data-ttu-id="9dd9e-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9dd9e-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9dd9e-117">description</span><span class="sxs-lookup"><span data-stu-id="9dd9e-117">description</span></span>|<span data-ttu-id="9dd9e-118">String</span><span class="sxs-lookup"><span data-stu-id="9dd9e-118">String</span></span>|<span data-ttu-id="9dd9e-119">说明。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-119">Description.</span></span> <span data-ttu-id="9dd9e-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9dd9e-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9dd9e-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="9dd9e-121">omaUri</span></span>|<span data-ttu-id="9dd9e-122">String</span><span class="sxs-lookup"><span data-stu-id="9dd9e-122">String</span></span>|<span data-ttu-id="9dd9e-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-123">OMA.</span></span> <span data-ttu-id="9dd9e-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9dd9e-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9dd9e-125">fileName</span><span class="sxs-lookup"><span data-stu-id="9dd9e-125">fileName</span></span>|<span data-ttu-id="9dd9e-126">String</span><span class="sxs-lookup"><span data-stu-id="9dd9e-126">String</span></span>|<span data-ttu-id="9dd9e-127">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="9dd9e-128">value</span><span class="sxs-lookup"><span data-stu-id="9dd9e-128">value</span></span>|<span data-ttu-id="9dd9e-129">Binary</span><span class="sxs-lookup"><span data-stu-id="9dd9e-129">Binary</span></span>|<span data-ttu-id="9dd9e-130">值。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-130">Value.</span></span> <span data-ttu-id="9dd9e-131">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="9dd9e-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd9e-132">关系</span><span class="sxs-lookup"><span data-stu-id="9dd9e-132">Relationships</span></span>
<span data-ttu-id="9dd9e-133">无</span><span class="sxs-lookup"><span data-stu-id="9dd9e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dd9e-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9dd9e-134">JSON Representation</span></span>
<span data-ttu-id="9dd9e-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dd9e-135">Here is a JSON representation of the resource.</span></span>
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
  "fileName": "String",
  "value": "binary"
}
```



