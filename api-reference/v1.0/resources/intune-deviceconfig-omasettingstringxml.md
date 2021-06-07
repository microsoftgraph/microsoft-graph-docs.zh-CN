---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6713977ef36edc43f1d2e00cf489f9906e6bd929
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755852"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="22dce-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="22dce-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="22dce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22dce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22dce-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22dce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22dce-106">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="22dce-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="22dce-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="22dce-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22dce-108">属性</span><span class="sxs-lookup"><span data-stu-id="22dce-108">Properties</span></span>
|<span data-ttu-id="22dce-109">属性</span><span class="sxs-lookup"><span data-stu-id="22dce-109">Property</span></span>|<span data-ttu-id="22dce-110">类型</span><span class="sxs-lookup"><span data-stu-id="22dce-110">Type</span></span>|<span data-ttu-id="22dce-111">说明</span><span class="sxs-lookup"><span data-stu-id="22dce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22dce-112">displayName</span><span class="sxs-lookup"><span data-stu-id="22dce-112">displayName</span></span>|<span data-ttu-id="22dce-113">String</span><span class="sxs-lookup"><span data-stu-id="22dce-113">String</span></span>|<span data-ttu-id="22dce-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="22dce-114">Display Name.</span></span> <span data-ttu-id="22dce-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="22dce-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="22dce-116">说明</span><span class="sxs-lookup"><span data-stu-id="22dce-116">description</span></span>|<span data-ttu-id="22dce-117">String</span><span class="sxs-lookup"><span data-stu-id="22dce-117">String</span></span>|<span data-ttu-id="22dce-118">说明。</span><span class="sxs-lookup"><span data-stu-id="22dce-118">Description.</span></span> <span data-ttu-id="22dce-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="22dce-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="22dce-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="22dce-120">omaUri</span></span>|<span data-ttu-id="22dce-121">String</span><span class="sxs-lookup"><span data-stu-id="22dce-121">String</span></span>|<span data-ttu-id="22dce-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="22dce-122">OMA.</span></span> <span data-ttu-id="22dce-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="22dce-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="22dce-124">fileName</span><span class="sxs-lookup"><span data-stu-id="22dce-124">fileName</span></span>|<span data-ttu-id="22dce-125">String</span><span class="sxs-lookup"><span data-stu-id="22dce-125">String</span></span>|<span data-ttu-id="22dce-126">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="22dce-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="22dce-127">value</span><span class="sxs-lookup"><span data-stu-id="22dce-127">value</span></span>|<span data-ttu-id="22dce-128">Binary</span><span class="sxs-lookup"><span data-stu-id="22dce-128">Binary</span></span>|<span data-ttu-id="22dce-129">值。</span><span class="sxs-lookup"><span data-stu-id="22dce-129">Value.</span></span> <span data-ttu-id="22dce-130">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="22dce-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="22dce-131">关系</span><span class="sxs-lookup"><span data-stu-id="22dce-131">Relationships</span></span>
<span data-ttu-id="22dce-132">无</span><span class="sxs-lookup"><span data-stu-id="22dce-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22dce-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22dce-133">JSON Representation</span></span>
<span data-ttu-id="22dce-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22dce-134">Here is a JSON representation of the resource.</span></span>
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




